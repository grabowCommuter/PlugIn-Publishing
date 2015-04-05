
##How to create a PlugIn for ACom?


To create a PlugIn, you have to perform three steps:

 **1. Develop the PlugIn:** You have to define the behavior of the PlugIn, that means define which script should be executed, which url
    should be loaded, etc. Our PlugIn-Developer-App will help you. (The
    app can be downloaded here).
    
 **2. Test the PlugIn:** Describe the behavior the the PlugIn in a JSON-Object and test the JSON-Object in our PlugIn-Tester (github:
    …).
    
 **3. Publish your PlugIn** (if you want to) on github.

---------

###Part 3: Publish the PlugIn

In **[Part 2: Test the PlugIn](https://github.com/grabowCommuter/PlugIn-Tester)** you have defined a PlugIn in form of a JSON-File. This PlugIn can be published on github the following way:

1. Create a new repository on github; the fullname of the repro will be the value of the  `moduleId` of your PlugIn. The name of the repro will be shown in the Search-List of ACom.

2. Put the string `(com.grabow.commuter.plugin)` somewhere into the description of the repro. ACom will search for repros containing this string in the description. 

3. If necessary, adjust the `moduleId`-value of your JSON-Object, so that it is equal to the  fullname of the github repro (e.g. `grabowCommuter/Speedometer` )

4. Save the PlugIn in the master-branch of your repro under the name `plugin.js`. Check the path to your PlugIn - it should be similar to the following example: `https://raw.githubusercontent.com/grabowCommuter/Speedometer/master/plugin.js`

5. Your done.

----
####Hint: 
- If you search and load the PlugIn via ACom, be aware that it takes some time (minutes) until the repro is published or updated on github.
- Android does cache downloaded files. If you reload your (even modified) PlugIn, Android might take the cached version. To check, which version is loaded select the „Edit PlugIn“ button and scroll to your PlugIn.
- Use the `README.md` file to explain what your PlugIn is good for. 
- Use the repro description to explain your PlugIn in short. Only the first 120 characters of the description will be shown in ACom. Don't forget to add the string `(com.grabow.commuter.plugin)`.


----

> Written with [StackEdit](https://stackedit.io/).
