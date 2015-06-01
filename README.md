# HTDroid
HTDroid is a protype system for detecting privacy leaks in Android hybrid apps based on dynamic taint tracking. More details about HTDroid can be found in the technical report.

##HTDroid System Architecture

HTDroid System is implemented based on [`TaintDroid`](http://appanalysis.org/index.html) and realizes the dynamic taint tracking function in `WebKit Engine` and `JavaScript Engine`.<br>
![](https://github.com/nwpufly/HTDroid/blob/master/HTDroid%20_System_Architecture.png)

### HTDroid Source Code Organization
| Code Project Name |    Comments                           |
|----- |---------|
| libnativehelper   | Modified the JNI header file          |
| dalvik VM         | Add GetStringTaint Function           |
| WebKit Engine     | Tracking String Taint Tag             |
| JavaScript Engine | Store String Taint Tag and Tracking<br>  taint propagation |



##How To Build!
* Build TaintDroid 4.3_r1 following the instruction [here](http://appanalysis.org/download.html).<br>
* 


##HTDroid Limitations
* Currently HTDroid System only supports tracking the String data following from Dalvik VM to WebKit Engine and JavaScript Engine.<br>
* 



