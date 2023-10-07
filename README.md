# A Mobile Application of Logic Education Based on AR
## Abstract
  With the rapid development of augmented reality technology in recent years, the application of mobile Ar has become more and more extensive. This paper introduces an AR mobile application based on AR Foundation which aims to popularize AR life style, let users experience the fun of AR. The project mainly through scanning the real plane, after the recognition is successful, the virtual object can be placed on the real world plane, and then the function operation can be carried out by clicking the corresponding button on the mobile phone screen, so as to realize the logic conversion. The original intention of the project is to let children combine hands-on ability and visual effects, so as to better realize the multi-dimensional development of intelligence.

## Keywords
  Human–Computer Interaction,AR,Unity,Education,Application,AR Foundation 

<p align="center">
  <img src ="https://github.com/30382716ZhiPang/AMobileApplicationofLogicEducationBasedonAR/assets/91645493/6594410e-8821-4f57-85fd-b0cdafb906ea" style="width: 800px"; alt="Sublime's custom"/>
<p>
 
<p align="center">
Fig. 1.	Screenshot of real-time operation
<p>
 
### I.	PROBLEM STATEMENT
  AR technology is a new technology that integrates the information of real world and virtual world.It uses computer and other science and technology to simulate the physical information that is difficult to experience in a certain time and space range of the real world, applies the virtual information to the real world, and is perceived by the human senses, so as to achieve the sensory experience beyond the reality.Real environment and virtual objects superimposed on the same picture or space in real time. AR system has real-time interaction, and users can interact with the system in many forms, thus creating a strong sense of immersion. AR technology can be widely used in military, medical, construction, education, engineering, film and television, entertainment and other fields.
With the development of smart phones and tablets, the application of mobile ar becomes more and more extensive. Arfoundation is an arkit XR plug-in（ com.unity.xr . arkit) and arcore XR plug-in（ com.unity.xr . arcore). Although the arkit SDK and arcore SDK are used in the end, the API called by C is slightly different from that of professional platforms (such as arkit plug-in and arcore SDK for unity) due to the re encapsulation of unity. Making full use of arfoundation, combining ar functions (such as plane detection, multi image recognition with interesting real scenes) and creating new ar playing methods (such as portal website and magic box), are highly interactive and interesting.

### II.	OUR NOVELTIES
A.	Based on ARFoundation Technology for Development
After studying the SDKs that can be used to implement AR function, we choose arfoundation (the development platform after unity encapsulates the third-party native SDKs such as arcore and arkit) so that unity developers can no longer be limited to a certain mobile platform for development, which can ensure that developers only need to develop applications once, and can be deployed to devices of two platforms, There is no need to make any changes.
This project is developed based on Android mobile terminal. Arfoundation inherits the adaptation of arcore for Android, and has a strong ability to perceive the environment, and can continuously improve the understanding of the real environment by detecting the feature points and the plane in the real scene. This project is based on the function of plane recognition to generate virtual plane objects as interactive scenes.
B.	AR technology combined with visual programming
The project scene is based on the switch between virtual and real environment. The virtual plane generated by AR technology is used as the interactive plane, and the role object is placed on the plane. After adding the condition and all the behaviors, the role will judge the execution according to the conditions The corresponding behavior that holds the behavior code block.
This mode of operation is different from the traditional visual programming for children's education. It effectively combines AR technology with traditional visual programming. On the basis of visual programming, it can give real-time feedback of virtual and real environment, increase the interest of user experience, and get rid of the boring stereotype of visual programming.

### III.	SYSTEM ARCHITECTURE
The system is divided into three modules: build scene, set parameters and run the program. Players first enter the main interactive interface, identify the plane through the scan plane button, click the select model button to select the character object and place it in the virtual plane, and then click the right scroll bar to select the "condition and behavior" module of the role, and set the conditions to determine the required parameters in the setting parameter button Finally, click the run program button, and the program will start to execute the code logic of all roles.
 
<p align="center">
  <img src ="https://github.com/30382716ZhiPang/AMobileApplicationofLogicEducationBasedonAR/assets/91645493/3d8ef4d4-e098-4c9b-b013-757af878912d"  style="width: 420px"; alt="Sublime's custom"/>
<p>

<p align="center">
Fig. 2.	System component
<p>
 
### IV.	TECHNICAL HIGHLIGHTS
In this project, the "code blocks" of conditions and all behaviors make use of task tasks thrown to threads. However, compared with thread pool, tasks require less overhead, and the control of "code blocks" in the project is more accurate and controllable. Each behavior "code block" is executed more than once, which means that the "code block" should be encapsulated and saved in the list by the way of delegation. Then, the unit's update function is used to judge whether there are tasks and continue to execute them. Thus, the thrown sub threads are returned to the unity main thread, and the behaviors in each role "code block" are gradually completed.
ACKNOWLEDGMENT

## Installation
When running an app integrated with the SDK, you need to ensure that SenseAR or OPPO ARUnit is installed on the device. As above
As shown in the table, some Xiaomi models and OPPO models have SenseAR or OPPO ARUnit pre-installed. And not
Pre-installed devices require manual installation of SenseAR. SenseAR is an apk file available on the SenseTime developer website
Download on. Since the integrated features are constantly updated, for developers who want to experience new features, we recommend using or replacing the pre-installed version
This upgrade to the latest SenseAR. Specific precautions are as follows:
① The name of Xiaomi’s pre-installed version of SenseAR in the application settings is ARServer, and the name of OPPO’s pre-installed version of SenseAR is
The name is ARUnit. The pre-installed version is relatively old and only contains the SLAM function. If you want to use more features, please update to the new version of SenseAR.
② The new version of SenseAR is continuously updated on the SenseTime developer website. After installation, the name of the application list is SenseAR. Use the new version.
The pre-installed version of SenseAR needs to be uninstalled first. The two cannot coexist, otherwise the application will not run properly.
③ In order to use the SenseAR SDK normally, you need to open the permission in SenseAR to allow other applications to start automatically, such as
As in OPPO mobile phones:
a) Application management->SenseAR->Allow other applications to start automatically,
b) Application Management->SenseAR->Power Consumption Protection->Allow background running. This step can be done after the subsequent SenseAR SDK upgrade.
to omit.

## Special thanks to Unity Technologies
<p align="center">
  <img src ="https://github.com/30382716ZhiPang/AMobileApplicationofLogicEducationBasedonAR/assets/91645493/48ee2c11-6b7d-4485-9b3e-9d26d4ad7db4"  style="width: 420px"; alt="Sublime's custom"/>
<p>
  
<p align="center">
Fig. 3.	Award certificate
<p>

This work was supported by the 20th ChinaVR conference and Connected Universal Experiences Laboratories.
REFERENCES

[1]	Modelling Player Preferences in AR Mobile Games. Vivek R. Warriar ; John R. Woodward ; Laurissa Tokarchuk. 2019 IEEE Conference on Games (CoG).

[2]	AR sightseeing system with proximity detection and markerless AR. Hidetaka Miyajima ; Noriko Yata ; Yoshitsugu Manabe. 2018 International Workshop on Advanced Image Technology (IWAIT).

[3]	An AR Benchmark System for Indoor Planar Object Tracking. Ziming Wu ; Jiabin Guo ; Shuangli Zhang ; Chen Zhao ; Xiaojuan Ma. 2019 IEEE International Conference on Multimedia and Expo (ICME).

[4]	A mobile visual programming system for Android smartphones and tablets. Wolfgang Slany. 2012 IEEE Symposium on Visual Languages and Human-Centric Computing (VL/HCC).

## Precautions
The copyright of the project belongs to the team. Secondary development or commercial use is prohibited without explicit authorization. This includes the use and distribution of source code, documentation, graphics, audio and other related materials. Violation of this provision may result in legal consequences. Please be sure to comply with intellectual property laws and related regulations.
