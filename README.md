Tomcat WebSockets Example
===

This example is designed for OpenShift and uses the `jbossews` [cartridge](https://github.com/openshift/origin-server/tree/master/cartridges/openshift-origin-cartridge-jbossews/README.md).

This example be tested by completing the following: 

```
rhc create-app -a APP_NAME -t jbossews-2.0

git remote add examples https://github.com/gssOpenShiftsupportExamples/Tomcat_WebSockets_Example.git
git fetch examples
git checkout master; git merge --strategy=recursive -X theirs examples/master
git push
```

This will push this example up to your openshift server for testing. You can then test the chat client with [http://APPNAME-NAMESPACE.rhcloud.com:8000/chat.html](http://APPNAME-NAMESPACE.rhcloud.com:8000/chat.html)
