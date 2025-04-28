# cs2030-lab-3--cruise-loaders-solved
**TO GET THIS SOLUTION VISIT:** [CS2030 Lab 3 # –Cruise Loaders Solved](https://www.ankitcodinghub.com/product/cs2030-lab-3-cruise-loaders-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;87166&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS2030 Lab 3 # –Cruise Loaders Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
&nbsp;

<h1>Task Content</h1>
<table width="680">
<tbody>
<tr>
<td width="680"><strong>Cruise Loaders Topic Coverage</strong>

Inheritance

Polymorphism

Method Overriding <a href="https://www.comp.nus.edu.sg/~cs2030/style/">CS2030 Java St</a><a href="https://www.comp.nus.edu.sg/~cs2030/style/">y</a><a href="https://www.comp.nus.edu.sg/~cs2030/style/">le Guide</a>

<strong>Problem Description</strong>

The Kent Ridge Cruise Centre has just opened and you are required to design a program to decide how many loaders to buy based on a single-day cruise schedule.

<strong>Cruises</strong>

Each cruise has four attributes:

a unique string identifier, e.g. S1234

a time of arrival in HHMM format, e.g. 2359 denoting the cruise arriving at 11:59PM on that day the time needed to serve the cruise (in minutes), and the number of loaders needed to serve the cruise.

Every cruise must be served by loaders immediately upon arrival.

There are two types of cruises:

SmallCruise:

has an identifier that starts with an uppercase character S; takes a fixed 30 minutes for a loader to fully load; requires only one loader for it to be fully served; BigCruise:

has an identifier that starts with an uppercase character B;

takes one minute to serve every 50 passengers; requires one loader per every 40 meters in length of the cruise (or part thereof) to fully load

<strong>Loaders</strong>

Loaders have to be purchased to serve cruises. Each loader comprises two attributes:

a unique integer identifier

the cruise that it is currently serving
</td>
</tr>
</tbody>
</table>
<table width="606">
<tbody>
<tr>
<td width="606">class Cruise {

private final String identifier;&nbsp;&nbsp;&nbsp;&nbsp; private final int arrivalTime;&nbsp;&nbsp;&nbsp;&nbsp; private final int numOfLoader;&nbsp;&nbsp;&nbsp;&nbsp; private final int serviceTime;

&nbsp;

… }
</td>
</tr>
</tbody>
</table>
A loader will serve a cruise as soon as it arrives, and continues to do so until the service time has elapsed (i.e. it cannot serve a cruise while in the midst of serving another one).

For example, if an incoming cruise arrives at 12PM, requires two loaders, and 60 min for it to be fully served, then, at 12PM, there must be two vacant loaders. These two loaders will serve the cruise from 12PM – 1PM. They can only serve another cruise from 1PM onwards.

<h1>Task</h1>
Your task is to determine the loader allocation schedule using the following steps:

For each cruise, check through the inventory of existing loaders, starting from the loader first purchased, and so on;

The first (or first few) loaders available will be used to serve the cruise;

If there are not enough loaders, purchase new one(s) to serve the cruise.

Take note of the following assumptions:

Input cruises are presented chronologically by arrival time.

There are no duplicate cruises.

All cruises will arrive and be completely served within a single day.

Although this problem can be implemented procedurally, you are to model your solution using an object-oriented approach instead.

This task is divided into several levels. You need to complete ALL levels.

<strong>Level 1</strong>

<h1>Represent a Cruise</h1>
Design an <em>immutable</em> Cruise class to represent a cruise having a unique identifier string, the time of arrival as an integer, the number of loaders required to load the cruise as an integer, and the service time in minutes as an integer.

Note that the time of arrival is in HHMM format. Specifically, 0 or 0000 refers to 00:00 (12AM), 30 or 0030 refers to 00:30 (12:30AM), and 130 or 0130 refers to 01:30 (1:30AM).

Implement a getServiceCompletionTime method, which returns the time the service completes (in number of minutes) since midnight, and a getArrivalTime method, which returns the arrival time (in number of minutes) since midnight.

For example, if the cruise arrives at 12PM (noon time), the arrival time is (12 * 60) = 720; the service completion time is 12:30PM, which is 750 minutes since midnight, i.e. (12 * 60) + 30 = 750.

In addition, implement a getNumOfLoadersRequired method, which returns the number of loaders required to load the cruise.

Tip: the %0Xd format specifier might be of use to you, where the integer will be represented by an X-digit zero-padded number. For instance,

String.format(“%04d”, 20);

would return the string 0020.

$ javac your_java_files

$ jshell your_java_files_in_bottom-up_dependency_order

jshell&gt; new Cruise(“A1234”, 0, 2, 30)

$.. ==&gt; A1234@0000

jshell&gt; new Cruise(“A2345”, 30, 2, 30)

$.. ==&gt; A2345@0030

jshell&gt; new Cruise(“A3456”, 130, 2, 30)

$.. ==&gt; A3456@0130

jshell&gt; new Cruise(“A3456”, 130, 2, 30).getArrivalTime() $.. ==&gt; 90

<table width="606">
<tbody>
<tr>
<td width="606">jshell&gt; new Cruise(“A3456”, 130, 2, 30).getNumOfLoadersRequired()

$.. ==&gt; 2

jshell&gt; new Cruise(“A3456”, 130, 5, 30).getNumOfLoadersRequired()

$.. ==&gt; 5

jshell&gt; new Cruise(“A1234”, 0, 2, 30).getServiceCompletionTime()

$.. ==&gt; 30

jshell&gt; new Cruise(“A1234”, 0, 2, 45).getServiceCompletionTime()

$.. ==&gt; 45

jshell&gt; new Cruise(“CS2030”, 1200, 2, 100).getServiceCompletionTime()

$.. ==&gt; 820

jshell&gt; new Cruise(“D1010”, 2329, 2, 30).getServiceCompletionTime()

$.. ==&gt; 1439 jshell&gt; /exit
</td>
</tr>
</tbody>
</table>
<table width="606">
<tbody>
<tr>
<td width="606">class Loader {

private final int identifier;&nbsp;&nbsp;&nbsp;&nbsp; private final Cruise cruise;

… }
</td>
</tr>
</tbody>
</table>
<table width="606">
<tbody>
<tr>
<td width="606">$ javac your_java_files

$ jshell your_java_files_in_bottom-up_dependency_order jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30))

$.. ==&gt; Loader 1 serving A1234@0000

jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30)).getIdentifier()

$.. ==&gt; 1

jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30)).getNextAvailableTime()

$.. ==&gt; 30

jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30)).canServe(new Cruise(“A2345”, 30, 1, 30))

$.. ==&gt; true

jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30)).serve(new Cruise(“A2345”, 30, 1, 30))

$.. ==&gt; Loader 1 serving A2345@0030

jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30)).serve(new Cruise(“A2345”, 30, 1, 30)).getNex

$.. ==&gt; 60

jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30)).canServe(new Cruise(“A2345”, 10, 1, 30))

$.. ==&gt; false

jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30)).serve(new Cruise(“A2345”, 10, 1, 30))

$.. ==&gt; Loader 1 serving A1234@0000

jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30)).serve(new Cruise(“A2345”, 10, 1, 30)).getNex

$.. ==&gt; 30

jshell&gt; new Loader(1, new Cruise(“A1234”, 0, 1, 30)).serve(new Cruise(“A2345”, 10, 1, 30)).getIde

$.. ==&gt; 1 jshell&gt; /exit
</td>
</tr>
</tbody>
</table>
<h1>Level 2</h1>
<h1>Use Loaders to serve Cruises</h1>
Design an <em>immutable</em> Loader class to serve a cruise.

Include the following in the Loader class:

a constructor that takes in an integer denoting its unique identifier, as well as the first cruise that it serves. a canServe(Cruise) method that returns true if the loader is available to serve the given cruise, or false otherwise.

a serve(Cruise) method to serve a given cruise. If the loader is available, the method returns the loader serving this cruise; otherwise the existing loader is returned the methods getIdentifier() and getNextAvailableTime() to return the loader’s identifier, and the next available time for service.

<strong>Level 3</strong>

<h1>Represent Small Cruises</h1>
Design the SmallCruise class. The arguments of the constructor are its identifier, and time of arrival. Note that you should not need to change your Loader class if you have implemented it properly.

$ javac your_java_files

<table width="606">
<tbody>
<tr>
<td width="606">$ javac your_java_files

$ jshell your_java_files_in_bottom-up_dependency_order jshell&gt; Cruise b = new BigCruise(“B0001”, 0, 70, 3000)

jshell&gt; b.getArrivalTime()

$.. ==&gt; 0

jshell&gt; b.getServiceCompletionTime()

$.. ==&gt; 60

jshell&gt; b.getNumOfLoadersRequired()

$.. ==&gt; 2

jshell&gt; new Loader(1, b).serve(b) $.. ==&gt; Loader 1 serving B0001@0000

jshell&gt; new Loader(1, b).serve(b).getNextAvailableTime()

$.. ==&gt; 60

jshell&gt; new Loader(2, b)

$.. ==&gt; Loader 2 serving B0001@0000 jshell&gt; new Loader(3, b)

$.. ==&gt; Loader 3 serving B0001@0000

jshell&gt; new Loader(4, new BigCruise(“B2345”, 0, 30, 1450)).serve(new SmallCruise(“S0000”, 29))

$.. ==&gt; Loader 4 serving S0000@0029

jshell&gt; new Loader(5, new BigCruise(“B3456”, 0, 75, 1510)).serve(new SmallCruise(“S0001”, 30))

$.. ==&gt; Loader 5 serving B3456@0000

jshell&gt; /exit
</td>
</tr>
</tbody>
</table>
<table width="606">
<tbody>
<tr>
<td width="606">$ javac your_java_files

$ jshell your_java_files_in_bottom-up_dependency_order

jshell&gt; List&lt;Cruise&gt; cruises = List.of(new SmallCruise(“S1111”, 1300))

cruises ==&gt; [S1111@1300]

&nbsp;

jshell&gt; serveCruises(cruises)

Loader 1 serving S1111@1300

&nbsp;

jshell&gt; cruises = List.of(new BigCruise(“B1111”, 1300, 80, 3000),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new SmallCruise(“S1111”, 1359),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new SmallCruise(“S1112”, 1400),&nbsp;&nbsp;&nbsp;&nbsp; …&gt;&nbsp;&nbsp;&nbsp;&nbsp; new SmallCruise(“S1113”, 1429))

cruises ==&gt; [B1111@1300, S1111@1359, S1112@1400, S1113@1429]

&nbsp;

jshell&gt; serveCruises(cruises) Loader 1 serving B1111@1300

Loader 2 serving B1111@1300
</td>
</tr>
</tbody>
</table>
$ jshell your_java_files_in_bottom-up_dependency_order jshell&gt; new SmallCruise(“S0001”, 0).getArrivalTime() $.. ==&gt; 0

jshell&gt; new SmallCruise(“S0001”, 0).getServiceCompletionTime()

$.. ==&gt; 30

jshell&gt; new SmallCruise(“S0001”, 0).getNumOfLoadersRequired()

$.. ==&gt; 1

jshell&gt; (Cruise) new SmallCruise(“S0123”, 1220)

$.. ==&gt; S0123@1220

jshell&gt; new Loader(1, new SmallCruise(“S1245”, 2330))

$.. ==&gt; Loader 1 serving S1245@2330

jshell&gt; new Loader(1, new SmallCruise(“S1245”, 2330)).canServe(new SmallCruise(“S2345”, 2359))

$.. ==&gt; false

jshell&gt; new Loader(1, new SmallCruise(“S1245”, 2330)).serve(new SmallCruise(“S2345”, 2359))

$.. ==&gt; Loader 1 serving S1245@2330

jshell&gt; new Loader(1, new SmallCruise(“S2030”, 0))

$.. ==&gt; Loader 1 serving S2030@0000 jshell&gt; /exit

<strong>Level 4</strong>

<h1>Represent Big Cruises</h1>
Design the BigCruise class. The arguments of the constructor are its identifier, time of arrival, the length of the cruise, and number of passengers, in that order.

<strong>Level 5</strong>

<h1>Output the loader allocation schedule</h1>
Write a method void serveCruises(List&lt;Cruise&gt; cruises) that takes in a list of cruises, and outputs the allocation schedule of the loaders required to service all the cruises. Save the method in the file level5.jsh.

&nbsp;

<table width="681">
<tbody>
<tr>
<td rowspan="2" width="37"></td>
<td width="607">Loader 3 serving S1111@1359

Loader 1 serving S1112@1400

Loader 2 serving S1113@1429

&nbsp;

jshell&gt; cruises = List.of(new SmallCruise(“S1111”, 900),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new BigCruise(“B1112”, 901, 100, 1),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new BigCruise(“B1113”, 902, 20, 4500),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new SmallCruise(“S2030”, 1031),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new BigCruise(“B0001”, 1100, 30, 1500),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new SmallCruise(“S0001”, 1130))

cruises ==&gt; [S1111@0900, B1112@0901, B1113@0902, S2030@1031, B0001@1100, S0001@1130]

&nbsp;

jshell&gt; serveCruises(cruises) Loader 1 serving S1111@0900

Loader 2 serving B1112@0901

Loader 3 serving B1112@0901

Loader 4 serving B1112@0901

Loader 2 serving B1113@0902

Loader 1 serving S2030@1031

Loader 2 serving B0001@1100

Loader 1 serving S0001@1130
</td>
<td rowspan="2" width="37"></td>
</tr>
<tr>
<td width="607"><strong>Level 6</strong>

<strong>Recycled Loaders</strong>

The objective of this level is to determine whether your current implementation can be easily extended with minimal modification to the client

The Cruise Centre has just introduced a new eco-friendly policy in an effort to go green. Their policy states that every third loader that is purchased must be made of recycled materials (referred to as recycled loaders). These recycled loaders will go through a 60-minute long maintenance after every service. It is unable to serve any cruise during this period.

For example, if a recycled loader serves a SmallCruise that arrives at 12:30PM, then the next time the loader can serve another Cruise is 2PM (30min + 60min after 12:30PM).

By modifying level5.jsh, incorporate the above with minimal modifications to the file level6.jsh.

<table width="606">
<tbody>
<tr>
<td width="606">$ javac your_java_files

$ jshell your_java_files_in_bottom-up_dependency_order

jshell&gt; List&lt;Cruise&gt; cruises = List.of(new BigCruise(“B1111”, 0, 60, 1500),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new SmallCruise(“S1112”, 0),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new BigCruise(“B1113”, 30, 100, 1500),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new BigCruise(“B1114”, 100, 100, 1500),

…&gt;&nbsp;&nbsp;&nbsp;&nbsp; new BigCruise(“B1115”, 130, 100, 1500),&nbsp;&nbsp;&nbsp; …&gt;&nbsp;&nbsp;&nbsp;&nbsp; new BigCruise(“B1116”, 200, 100, 1500))

cruises ==&gt; [B1111@0000, S1112@0000, B1113@0030, B1114@0100, B1115@0130, B1116@0200]

&nbsp;

jshell&gt; serveCruises(cruises) Loader 1 serving B1111@0000

Loader 2 serving B1111@0000

Recycled Loader 3 serving S1112@0000

Loader 1 serving B1113@0030

Loader 2 serving B1113@0030

Loader 4 serving B1113@0030

Loader 1 serving B1114@0100

Loader 2 serving B1114@0100

Loader 4 serving B1114@0100

Loader 1 serving B1115@0130

Loader 2 serving B1115@0130

Recycled Loader 3 serving B1115@0130

Loader 1 serving B1116@0200

Loader 2 serving B1116@0200

Loader 4 serving B1116@0200
</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td colspan="3" width="681"></td>
</tr>
</tbody>
</table>
&nbsp;
