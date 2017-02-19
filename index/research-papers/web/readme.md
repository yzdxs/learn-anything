#[research papers - web](https://my.mindnode.com/Kkam7na79qaY1Vn41gpwbzV1tW5DpJzSHyryLWKM)

![](http://i.imgur.com/7jaH88Q.png)

#mindmap index 🗄️

# [DOPPIO: Breaking the Browser Language Barrier ✨](http://plasma-umass.github.io/doppio-demo/paper.pdf)


## intro

### DOPPIO, a JavaScript-based runtime system that makes it possible to run unaltered applications written in general- purpose languages directly inside the browser.

- provides a wide range of runtime services, including a ﬁle system that enables local and external (cloud-based) storage, an unmanaged heap, sockets, blocking I/O, and multiple threads.

### Browsers make it comparatively easy to deliver cross-platform applications, because they are effectively ubiquitous.

- Browsers are also getting faster.

- Most now incorporate optimising just-in-time compilers for JavaScript, and expose features like access to the GPU through WebGL and high-speed video chat via WebRTC

	- This combination of features makes it possible for browsers to host the kind of richly interactive applications that used to be restricted to native environments.

### web browsers have become a de facto universal computing platform: its operating system is the browser environment, and its sole “instruction set” is JavaScript.

- However, running languages other than JavaScript in the browser is not generally possible.

### Programmers who prefer to program in other paradigms (e.g., functional, object-oriented) currently must abandon these or build hacks onto JavaScript to accomodate their needs.

- There is also a vast body of well-debugged, existing code written in general-purpose pro- gramming languages.

- Making it possible to reuse this code, rather than requiring that it all be re-written in JavaScript, would speed application development and reduce the risk of introducing errors.

### Translation, interpretation, or compilation of languages to JavaScript is necessary but not sufﬁcient.

- Browsers lack many key abstractions that existing programming languages expect, impose signiﬁcant limitations, and vary widely in their support for and compliance with standards:

	- **Single-threaded Execution**:

		- JavaScript is a single-threaded event-driven programming language with no support for interrupts.

		- Events either execute to completion, or until they are killed by the browser’s watchdog thread because they took too long to ﬁnish.

	- **Asynchronous-only APIs**:

		- Browsers provide web applications with a rich set of functionality, but emerging APIs are exclusively asynchronous.

		- Due to the limitations of JavaScript, it is not possible to create synchronous APIs from asynchronous APIs.

	- **Missing OS Services**:

		- Browsers do not provide applications with access to a ﬁle system abstraction.

		- Instead, they offer a panoply of limited persistent storage mechanisms, making it difﬁcult to manage large amounts of persistent data.

		- Browsers also lack other OS services such as sockets.

	- **Browser Diversity**:

		- Users access the web from a wide range of browser platforms, operating systems, and devices.

		- Each combi- nation may have unique performance characteristics, differing support for JavaScript and Document Object Model (DOM) features, and outright bugs.

		- This diversity makes it difﬁcult to address any of the issues above without excluding a large portion of the web audience.

### Feature comparison of systems that execute existing code inside the browser. The asterisk and dagger indicate limitations that prevent execution on browsers used by over half of the web population today: “∗” denotes a feature that requires a (non-default) backwards- compatibility ﬂag in order to work in those browsers, while a “†” indicates that the feature will not work for them [3]. D OPPIO and the D OPPIO JVM implement all of these features in a cross-platform approach, letting it run unmodiﬁed programs in the vast majority of browsers.

## related work

### One of the most prominent and earliest implementations of conventional languages inside the browser is Google Web Toolkit (GWT), a source-to-source compiler from Java to JavaScript

- The goal of GWT is to let web developers write AJAX web applications using a restricted subset of Java.

### FINISH: 

