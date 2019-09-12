# liferay-js-toolkit-demo

## my-project
npx create-react-app my-project
yo liferay-js:adapt (2.13.0)
deploy to Liferay DXP 7.2.10 GA 1...

### from the server console (after deploying):
2019-09-12 12:53:49.695 INFO  [com.liferay.portal.kernel.deploy.auto.AutoDeployScanner][AutoDeployDir:261] Processing my-project-0.1.0.jar
2019-09-12 12:53:58.336 INFO  [fileinstall-C:/liferay/liferay-dxp-7.2.10-ga1/osgi/modules][BundleStartStopLogger:39] STARTED my-project_0.1.0 [2210]

### from the server console (after adding to a page):
2019-09-12 12:54:56.925 WARN  [http-nio-8080-exec-10][code_jsp:?] {code="404", msg="ProxyServlet: /my-project-0.1.0react-app/static/css/main.2cce8147.chunk.css.map", uri=/o/my-project-0.1.0react-app/static/css/main.2cce8147.chunk.css.map}

### from the browser console (after adding to a page):
Liferay AMD Loader: Require call 2 resolved modules ["my-project@0.1.0"] to {pathMap: {…}, configMap: {…}, resolvedModules: Array(1), moduleMap: {…}}
loader.js:369 Liferay AMD Loader: Invoking failure handler for require call 2
loader.js:222 ---------------------------------------
loader.js:223 Liferay AMD Loader: Unhandled require failure:
loader.js:224 
NOTE: You are seeing this message because you have
invoked require() without a failure handler. It
does not necessarily mean that the Loader is
broken and may be caused by errors in your code or
third party modules.

If you want to avoid it make sure to provide a
failure handler when calling require().


loader.js:233 A detailed report of what happened follows:
loader.js:234   · Require call id: 2
loader.js:235   · Required modules: ["my-project@0.1.0"]
loader.js:236   · Error cause: Error: The following problems where detected while resolving modules:
    · Missing required module 'my-project@0.1.0'
    at e.value (loader.js:421)
    at loader.js:265
loader.js:240   · Caller's stack trace: Error: This is not a real error, but a fake one created to capture require()'s caller stack trace
    at e.value (loader.js:212)
    at <anonymous>:58:17
    at Object.addHTML (dom-base.js:518)
    at Y_Node._insert (node-base.js:180)
    at Y_Node.appendChild (node-base.js:217)
    at component.globalEval (aui-parse-content.js:159)
    at Y.AsyncQueue.<anonymous> (async-queue.js:201)
    at Y.EventFacade.callback (oop.js:403)
    at Y.AsyncQueue._defExecFn (async-queue.js:318)
    at Y.CustomEvent.CEProto.fireComplex (event-custom-complex.js:337)
