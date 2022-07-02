DayZ Chernarus Compatible Code To Return Loot To Small Green Guard Watch Towers xml Snippet Mod Changelog & Terms Of Use

Limited Testing on PC Chernarus Local Server DAYZ Version 1.18 July 2022.

Created by @scalespeeder. Please report bugs & errors to scalespeeder@gmail.com with screenshots.

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded xml files could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded xml files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

To re-activate loot spawns in the small green guard towers often found around military locations, take the following steps.

Stop your server. Download and edit or open in your webbrowser the mapgroupproto.xml file, which is found inside your servers mission folder.

After the </defaults> entry on approx line 17, copy and paste the following xml snippet: 

	<!--mapgroupproto.xml small guard tower xml snippet-->
	<group name="Land_Mil_Tower_Small" lootmax="2">
				<usage name="Military" />
				<container name="lootFloor" lootmax="2">
						<category name="clothes" />
						<category name="weapons" />
						<category name="explosives" />
						<point height="1.114502" range="0.445802" pos="1.538687 1.277588 0.398074"/>
						<point height="0.973297" range="0.416016" pos="0.955226 1.277588 -0.327999"/>
				</container>
		</group>
	
	<!--end of mapgroupproto.xml small guard tower xml snippet-->
	
Save your edited mapgroupproto.xml and re-upload if necessary.

Next, download and edit or open in your webbrowser the mapgrouppos.xml file, which is found inside your servers mission folder.

Near the top, underneath the <map> entry, copy and paste the following xml snippet: 
	
	<!--mapgrouppos.xml small guard tower xml snippet-->
	<group name="Land_Mil_Tower_Small" pos="1014.983582 474.824707 13894.623047" rpy="-0.000000 0.000000 -125.433807" a="-144.566177" />
    <group name="Land_Mil_Tower_Small" pos="1850.564087 136.789307 3544.727539" rpy="0.027297 -0.006128 12.652076" a="77.347923" />
    <group name="Land_Mil_Tower_Small" pos="1906.949219 125.552040 3377.714844" rpy="-0.000000 0.000000 -152.762665" a="-117.237320" />
    <group name="Land_Mil_Tower_Small" pos="2012.453247 109.297676 3240.803955" rpy="-0.014121 0.013853 -135.549133" a="-134.450867" />
    <group name="Land_Mil_Tower_Small" pos="2061.879150 97.862083 3283.748535" rpy="-0.000000 0.000000 -84.921394" a="174.921402" />
    <group name="Land_Mil_Tower_Small" pos="2053.483398 113.897392 3378.123291" rpy="-0.000000 0.000000 -75.552147" a="165.552155" />
    <group name="Land_Mil_Tower_Small" pos="2059.571045 115.787750 3416.119629" rpy="0.023358 0.015397 -33.392262" a="123.392250" />
    <group name="Land_Mil_Tower_Small" pos="2057.072510 128.673569 3640.294922" rpy="0.019765 -0.000825 2.389251" a="87.610741" />
    <group name="Land_Mil_Tower_Small" pos="2107.638428 98.163956 3404.383301" rpy="-0.000000 0.000000 -5.672052" a="95.672043" />
    <group name="Land_Mil_Tower_Small" pos="2167.415771 90.714569 3271.960693" rpy="-0.000000 0.000000 -175.326035" a="-94.673950" />
    <group name="Land_Mil_Tower_Small" pos="2205.937500 90.892578 3241.312744" rpy="-0.018363 -0.007357 158.168076" a="-68.168083" />
    <group name="Land_Mil_Tower_Small" pos="2190.254883 97.830116 3406.873291" rpy="0.018594 -0.006751 19.953697" a="70.046295" />
    <group name="Land_Mil_Tower_Small" pos="2208.861816 129.837494 3634.812256" rpy="-0.000000 0.000000 -24.844364" a="114.844368" />
    <group name="Land_Mil_Tower_Small" pos="2255.992676 98.016411 3261.023193" rpy="-0.000000 0.000000 168.234528" a="-78.234535" />
    <group name="Land_Mil_Tower_Small" pos="2249.112793 102.344101 3386.370117" rpy="-0.000000 0.000000 10.992988" a="79.007004" />
    <group name="Land_Mil_Tower_Small" pos="2322.641602 94.188789 3192.437256" rpy="-0.000000 0.000000 127.827477" a="-37.827480" />
    <group name="Land_Mil_Tower_Small" pos="2357.901123 131.273758 3427.373779" rpy="-0.043294 -0.035445 140.693115" a="-50.693127" />
    <group name="Land_Mil_Tower_Small" pos="2378.029541 192.980530 5130.334961" rpy="-0.000000 0.000000 -101.062363" a="-168.937637" />
    <group name="Land_Mil_Tower_Small" pos="2440.833984 136.393967 3575.078125" rpy="-0.000000 0.000000 41.673504" a="48.326488" />
    <group name="Land_Mil_Tower_Small" pos="2447.429199 196.918671 5112.831543" rpy="-0.000000 0.000000 -130.267334" a="-139.732651" />
    <group name="Land_Mil_Tower_Small" pos="2432.954346 194.255066 5184.279297" rpy="-0.000000 0.000000 -21.728514" a="111.728508" />
    <group name="Land_Mil_Tower_Small" pos="2506.088135 197.654251 5034.263184" rpy="-0.023861 -0.014606 148.528076" a="-58.528080" />
    <group name="Land_Mil_Tower_Small" pos="2466.996826 196.647903 5085.598633" rpy="-0.000000 0.000000 -123.625389" a="-146.374588" />
    <group name="Land_Mil_Tower_Small" pos="2484.139893 197.087646 5060.107910" rpy="-0.015120 0.023538 -122.715462" a="-147.284531" />
    <group name="Land_Mil_Tower_Small" pos="2510.300781 194.271637 5198.384766" rpy="-0.000000 0.000000 -8.560211" a="98.560204" />
    <group name="Land_Mil_Tower_Small" pos="2546.973633 23.562983 1329.544800" rpy="-0.000000 0.000000 -79.764023" a="169.764023" />
    <group name="Land_Mil_Tower_Small" pos="2545.966309 197.337311 5094.734863" rpy="-0.023820 -0.014672 148.369217" a="-58.369221" />
    <group name="Land_Mil_Tower_Small" pos="2562.957275 194.181030 5205.895508" rpy="-0.000000 0.000000 -8.560211" a="98.560204" />
    <group name="Land_Mil_Tower_Small" pos="2599.267822 198.589005 5151.560059" rpy="-0.000000 0.000000 87.831703" a="2.168296" />
    <group name="Land_Mil_Tower_Small" pos="2598.032715 199.143356 5185.655762" rpy="-0.000000 0.000000 84.890297" a="5.109696" />
    <group name="Land_Mil_Tower_Small" pos="2657.484131 27.107624 1309.302246" rpy="-0.000000 0.000000 100.550934" a="-10.550937" />
    <group name="Land_Mil_Tower_Small" pos="2644.197021 26.502441 1327.407959" rpy="-0.000000 0.000000 -80.279709" a="170.279709" />
    <group name="Land_Mil_Tower_Small" pos="2758.663818 29.728222 1238.761230" rpy="-0.000000 0.000000 -144.678879" a="-125.321114" />
    <group name="Land_Mil_Tower_Small" pos="2710.408936 27.014809 1299.922607" rpy="0.006970 0.038946 -79.853722" a="169.853714" />
    <group name="Land_Mil_Tower_Small" pos="2803.920654 29.738590 1196.207520" rpy="-0.033742 0.028605 -139.709778" a="-130.290207" />
    <group name="Land_Mil_Tower_Small" pos="2769.312988 29.727951 1225.973755" rpy="-0.033579 0.028796 -139.384735" a="-130.615265" />
    <group name="Land_Mil_Tower_Small" pos="2828.021240 29.745543 1217.915527" rpy="-0.036876 0.031437 -139.552048" a="-130.447952" />
    <group name="Land_Mil_Tower_Small" pos="3526.246582 336.248230 11551.173828" rpy="-0.000000 0.000000 -113.002510" a="-156.997482" />
    <group name="Land_Mil_Tower_Small" pos="3516.653564 329.913788 11627.990234" rpy="-0.000000 0.000000 -53.892830" a="143.892838" />
    <group name="Land_Mil_Tower_Small" pos="3574.269775 331.854065 10917.599609" rpy="-0.000000 0.000000 -100.646461" a="-169.353531" />
    <group name="Land_Mil_Tower_Small" pos="3582.207031 331.420807 11338.868164" rpy="-0.000000 0.000000 -121.559097" a="-148.440887" />
    <group name="Land_Mil_Tower_Small" pos="3563.295166 333.569458 11380.521484" rpy="-0.000000 0.000000 -86.550179" a="176.550171" />
    <group name="Land_Mil_Tower_Small" pos="3565.531250 340.773041 11472.711914" rpy="-0.000000 0.000000 -117.860443" a="-152.139542" />
    <group name="Land_Mil_Tower_Small" pos="3596.099121 332.338104 11708.261719" rpy="-0.000000 0.000000 -44.806683" a="134.806686" />
    <group name="Land_Mil_Tower_Small" pos="3648.366699 337.512543 10858.781250" rpy="-0.000000 0.000000 -136.116379" a="-133.883606" />
    <group name="Land_Mil_Tower_Small" pos="3633.630859 323.314056 10981.434570" rpy="-0.000000 0.000000 -57.196346" a="147.196350" />
    <group name="Land_Mil_Tower_Small" pos="3643.415527 319.098328 11085.870117" rpy="-0.000000 0.000000 -119.224098" a="-150.775879" />
    <group name="Land_Mil_Tower_Small" pos="3609.115479 319.744354 11163.717773" rpy="-0.000000 0.000000 -36.779305" a="126.779297" />
    <group name="Land_Mil_Tower_Small" pos="3605.693115 323.892487 11234.815430" rpy="-0.000000 0.000000 -96.790955" a="-173.209045" />
    <group name="Land_Mil_Tower_Small" pos="3711.551270 340.018829 10785.837891" rpy="-0.000000 0.000000 -124.388649" a="-145.611328" />
    <group name="Land_Mil_Tower_Small" pos="3671.637695 327.105774 11779.085938" rpy="-0.000000 0.000000 -47.592941" a="137.592941" />
    <group name="Land_Mil_Tower_Small" pos="3696.783447 313.989563 11890.065430" rpy="-0.000000 0.000000 -55.554203" a="145.554199" />
    <group name="Land_Mil_Tower_Small" pos="3760.570068 346.913971 10629.483398" rpy="-0.000000 0.000000 -98.387634" a="-171.612366" />
    <group name="Land_Mil_Tower_Small" pos="3760.864990 346.147919 10702.005859" rpy="-0.000000 0.000000 -105.515999" a="-164.483994" />
    <group name="Land_Mil_Tower_Small" pos="3816.281006 353.259949 10449.052734" rpy="-0.000000 0.000000 -106.685356" a="-163.314636" />
    <group name="Land_Mil_Tower_Small" pos="3782.009033 348.361176 10564.865234" rpy="-0.000000 0.000000 -106.682320" a="-163.317673" />
    <group name="Land_Mil_Tower_Small" pos="3785.563232 307.368835 11965.131836" rpy="-0.000000 0.000000 -42.463436" a="132.463440" />
    <group name="Land_Mil_Tower_Small" pos="3865.198486 355.002014 10368.464844" rpy="-0.000000 0.000000 -129.181366" a="-140.818619" />
    <group name="Land_Mil_Tower_Small" pos="3857.279297 301.045532 12015.688477" rpy="-0.000000 0.000000 -31.415607" a="121.415611" />
    <group name="Land_Mil_Tower_Small" pos="3926.209229 354.346252 10286.111328" rpy="-0.000000 0.000000 -122.848633" a="-147.151352" />
    <group name="Land_Mil_Tower_Small" pos="3948.612793 298.636292 12071.765625" rpy="-0.000000 0.000000 -16.938450" a="106.938446" />
    <group name="Land_Mil_Tower_Small" pos="4007.168457 349.071320 10182.907227" rpy="-0.000000 0.000000 -150.325424" a="-119.674568" />
    <group name="Land_Mil_Tower_Small" pos="3970.882080 372.897583 11678.173828" rpy="-0.000000 0.000000 -123.598320" a="-146.401672" />
    <group name="Land_Mil_Tower_Small" pos="3977.084473 379.195007 11769.750000" rpy="-0.000000 0.000000 -135.747345" a="-134.252640" />
    <group name="Land_Mil_Tower_Small" pos="3965.577148 378.428528 11849.476563" rpy="-0.000000 0.000000 -87.919273" a="177.919281" />
    <group name="Land_Mil_Tower_Small" pos="3990.560059 378.870972 11896.010742" rpy="-0.000000 0.000000 -5.640824" a="95.640816" />
    <group name="Land_Mil_Tower_Small" pos="4041.140625 371.868408 11576.648438" rpy="-0.000000 0.000000 -150.518372" a="-119.481613" />
    <group name="Land_Mil_Tower_Small" pos="4048.644043 378.963623 11873.968750" rpy="-0.000000 0.000000 12.910016" a="77.089981" />
    <group name="Land_Mil_Tower_Small" pos="4053.401611 294.992188 12076.540039" rpy="-0.000000 0.000000 14.880892" a="75.119102" />
    <group name="Land_Mil_Tower_Small" pos="4122.055664 346.562408 10164.566406" rpy="-0.000000 0.000000 -123.862511" a="-146.137482" />
    <group name="Land_Mil_Tower_Small" pos="4170.045898 342.626587 10091.126953" rpy="-0.000000 0.000000 -121.290504" a="-148.709473" />
    <group name="Land_Mil_Tower_Small" pos="4172.079590 290.059723 12045.607422" rpy="-0.000000 0.000000 31.441416" a="58.558582" />
    <group name="Land_Mil_Tower_Small" pos="4219.350098 343.684479 10021.766602" rpy="-0.000000 0.000000 -153.425171" a="-116.574821" />
    <group name="Land_Mil_Tower_Small" pos="4241.939941 290.358734 11978.536133" rpy="-0.000000 0.000000 45.497227" a="44.502769" />
    <group name="Land_Mil_Tower_Small" pos="4332.339355 342.426178 10015.502930" rpy="-0.000000 0.000000 -178.951508" a="-91.048470" />
    <group name="Land_Mil_Tower_Small" pos="4320.751465 291.621826 11897.700195" rpy="-0.000000 0.000000 42.658810" a="47.341183" />
    <group name="Land_Mil_Tower_Small" pos="4390.272949 341.756561 9541.070313" rpy="-0.000000 0.000000 -109.149582" a="-160.850418" />
    <group name="Land_Mil_Tower_Small" pos="4388.489258 342.477448 9619.158203" rpy="-0.000000 0.000000 -78.175110" a="168.175110" />
    <group name="Land_Mil_Tower_Small" pos="4431.695801 304.380219 11536.471680" rpy="-0.000000 0.000000 80.872284" a="9.127711" />
    <group name="Land_Mil_Tower_Small" pos="4425.675293 298.699524 11635.101563" rpy="-0.000000 0.000000 88.773590" a="1.226406" />
    <group name="Land_Mil_Tower_Small" pos="4416.967285 295.805695 11697.063477" rpy="-0.000000 0.000000 63.770706" a="26.229288" />
    <group name="Land_Mil_Tower_Small" pos="4397.411133 288.562195 11813.101563" rpy="-0.000000 0.000000 71.623520" a="18.376476" />
    <group name="Land_Mil_Tower_Small" pos="4483.811523 342.502014 9743.993164" rpy="-0.000000 0.000000 -52.718746" a="142.718750" />
    <group name="Land_Mil_Tower_Small" pos="4447.778809 343.844177 10009.959961" rpy="-0.000000 0.000000 -155.891327" a="-114.108650" />
    <group name="Land_Mil_Tower_Small" pos="4464.931152 306.805878 11336.441406" rpy="-0.000000 0.000000 67.613579" a="22.386412" />
    <group name="Land_Mil_Tower_Small" pos="4445.470703 304.494720 11453.477539" rpy="-0.000000 0.000000 83.206825" a="6.793167" />
    <group name="Land_Mil_Tower_Small" pos="4528.770020 343.017029 9829.278320" rpy="-0.000000 0.000000 -72.324966" a="162.324966" />
    <group name="Land_Mil_Tower_Small" pos="4527.261230 343.087433 9899.904297" rpy="-0.000000 0.000000 -101.807129" a="-168.192871" />
    <group name="Land_Mil_Tower_Small" pos="4557.199219 305.176910 11207.123047" rpy="-0.000000 0.000000 48.944427" a="41.055569" />
    <group name="Land_Mil_Tower_Small" pos="4593.781250 322.484985 8230.234375" rpy="-0.027513 -0.005068 169.563919" a="-79.563919" />
    <group name="Land_Mil_Tower_Small" pos="4578.540039 322.198303 8373.045898" rpy="-0.000000 0.000000 4.304615" a="85.695381" />
    <group name="Land_Mil_Tower_Small" pos="4577.953613 342.638580 9364.256836" rpy="-0.000000 0.000000 -155.149811" a="-114.850174" />
    <group name="Land_Mil_Tower_Small" pos="4644.123047 343.959045 9292.021484" rpy="-0.000000 0.000000 -146.124069" a="-123.875908" />
    <group name="Land_Mil_Tower_Small" pos="4672.237793 299.757751 11143.849609" rpy="-0.000000 0.000000 45.208767" a="44.791225" />
    <group name="Land_Mil_Tower_Small" pos="4721.891113 347.063873 9241.060547" rpy="-0.000000 0.000000 -143.041061" a="-126.958923" />
    <group name="Land_Mil_Tower_Small" pos="4715.024902 305.604095 11081.584961" rpy="-0.000000 0.000000 44.611294" a="45.388702" />
    <group name="Land_Mil_Tower_Small" pos="4790.660645 347.950531 9163.302734" rpy="-0.000000 0.000000 -129.289642" a="-140.710342" />
    <group name="Land_Mil_Tower_Small" pos="4781.810059 315.877228 11009.306641" rpy="-0.000000 0.000000 60.264202" a="29.735790" />
    <group name="Land_Mil_Tower_Small" pos="4854.124023 347.588379 9100.768555" rpy="-0.000000 0.000000 -149.980927" a="-120.019051" />
    <group name="Land_Mil_Tower_Small" pos="4820.478027 323.237762 10936.613281" rpy="-0.000000 0.000000 60.264202" a="29.735794" />
    <group name="Land_Mil_Tower_Small" pos="4910.131348 337.900513 10557.164063" rpy="-0.000000 0.000000 80.558121" a="9.441873" />
    <group name="Land_Mil_Tower_Small" pos="4896.608398 332.498291 10656.949219" rpy="-0.000000 0.000000 88.290001" a="1.709997" />
    <group name="Land_Mil_Tower_Small" pos="4892.839844 330.281311 10740.481445" rpy="-0.000000 0.000000 84.160866" a="5.839133" />
    <group name="Land_Mil_Tower_Small" pos="4872.552734 326.666687 10845.925781" rpy="-0.000000 0.000000 61.504524" a="28.495470" />
    <group name="Land_Mil_Tower_Small" pos="4943.360352 352.234283 9073.015625" rpy="-0.000000 0.000000 -161.092819" a="-108.907166" />
    <group name="Land_Mil_Tower_Small" pos="4940.449707 337.188171 10381.017578" rpy="-0.000000 0.000000 62.357151" a="27.642843" />
    <group name="Land_Mil_Tower_Small" pos="5014.129395 354.043640 9046.877930" rpy="-0.000000 0.000000 -157.849564" a="-112.150406" />
    <group name="Land_Mil_Tower_Small" pos="4985.472168 333.976074 10302.146484" rpy="-0.000000 0.000000 36.881348" a="53.118649" />
    <group name="Land_Mil_Tower_Small" pos="5081.140625 354.940247 9022.610352" rpy="-0.000000 0.000000 161.442474" a="-71.442482" />
    <group name="Land_Mil_Tower_Small" pos="5073.680664 328.876526 10263.163086" rpy="-0.000000 0.000000 -16.086205" a="106.086197" />
    <group name="Land_Mil_Tower_Small" pos="5117.095215 355.307739 9076.527344" rpy="-0.000000 0.000000 114.339699" a="-24.339705" />
    <group name="Land_Mil_Tower_Small" pos="5141.426758 354.316956 9127.259766" rpy="-0.000000 0.000000 124.376396" a="-34.376404" />
    <group name="Land_Mil_Tower_Small" pos="5180.573730 352.873322 9177.377930" rpy="-0.000000 0.000000 124.376396" a="-34.376404" />
    <group name="Land_Mil_Tower_Small" pos="5209.807617 349.654358 9229.165039" rpy="-0.000000 0.000000 114.145432" a="-24.145437" />
    <group name="Land_Mil_Tower_Small" pos="5177.578613 317.114349 10295.266602" rpy="-0.000000 0.000000 3.619581" a="86.380417" />
    <group name="Land_Mil_Tower_Small" pos="5234.895020 345.865906 9294.919922" rpy="-0.000000 0.000000 110.539642" a="-20.539644" />
    <group name="Land_Mil_Tower_Small" pos="5276.495117 343.753143 9351.738281" rpy="-0.000000 0.000000 158.633728" a="-68.633736" />
    <group name="Land_Mil_Tower_Small" pos="5258.177246 345.043640 9434.018555" rpy="-0.000000 0.000000 89.901649" a="0.098345" />
    <group name="Land_Mil_Tower_Small" pos="5276.046875 344.115387 9535.646484" rpy="-0.000000 0.000000 103.387352" a="-13.387357" />
    <group name="Land_Mil_Tower_Small" pos="5261.134766 318.333557 10197.211914" rpy="-0.000000 0.000000 42.077415" a="47.922577" />
    <group name="Land_Mil_Tower_Small" pos="5329.515625 342.303467 9625.181641" rpy="-0.000000 0.000000 125.322273" a="-35.322273" />
    <group name="Land_Mil_Tower_Small" pos="5335.483887 320.097046 10132.222656" rpy="-0.000000 0.000000 42.194237" a="47.805763" />
    <group name="Land_Mil_Tower_Small" pos="5386.528809 338.798645 9676.723633" rpy="-0.000000 0.000000 118.802826" a="-28.802834" />
    <group name="Land_Mil_Tower_Small" pos="5394.759277 321.848816 10074.377930" rpy="-0.000000 0.000000 70.737434" a="19.262564" />
    <group name="Land_Mil_Tower_Small" pos="5424.094238 332.602570 9788.995117" rpy="-0.000000 0.000000 101.433601" a="-11.433609" />
    <group name="Land_Mil_Tower_Small" pos="5443.744629 333.726074 9905.070313" rpy="-0.000000 0.000000 97.485168" a="-7.485171" />
    <group name="Land_Mil_Tower_Small" pos="5422.260254 327.619995 9998.682617" rpy="-0.000000 0.000000 70.737434" a="19.262564" />
    <group name="Land_Mil_Tower_Small" pos="7641.868652 371.885223 14842.642578" rpy="-0.000000 0.000000 -89.187698" a="179.187698" />
    <group name="Land_Mil_Tower_Small" pos="7732.367676 335.301392 14597.585938" rpy="-0.000000 0.000000 -132.552750" a="-137.447235" />
    <group name="Land_Mil_Tower_Small" pos="7710.191406 346.872284 14668.786133" rpy="-0.000000 0.000000 -113.054176" a="-156.945816" />
    <group name="Land_Mil_Tower_Small" pos="7681.019043 357.325287 14738.452148" rpy="-0.000000 0.000000 -109.148865" a="-160.851120" />
    <group name="Land_Mil_Tower_Small" pos="7724.562500 364.596344 14804.835938" rpy="-0.034259 0.000586 -179.020401" a="-90.979584" />
    <group name="Land_Mil_Tower_Small" pos="7702.754395 382.743561 14930.512695" rpy="0.025448 0.022944 -42.037476" a="132.037460" />
    <group name="Land_Mil_Tower_Small" pos="7793.125000 326.473419 14532.805664" rpy="-0.026508 0.035413 -126.816910" a="-143.183075" />
    <group name="Land_Mil_Tower_Small" pos="7798.800781 388.764221 14940.840820" rpy="0.032505 -0.010838 18.440145" a="71.559845" />
    <group name="Land_Mil_Tower_Small" pos="7846.301758 321.098053 14500.860352" rpy="-0.000000 0.000000 -176.578033" a="-93.421951" />
    <group name="Land_Mil_Tower_Small" pos="7832.466797 334.640045 14587.111328" rpy="-0.028263 -0.019371 145.573639" a="-55.573658" />
    <group name="Land_Mil_Tower_Small" pos="7840.872559 369.760406 14857.774414" rpy="-0.000000 0.000000 65.639740" a="24.360256" />
    <group name="Land_Mil_Tower_Small" pos="7894.788574 340.576141 14609.654297" rpy="-0.039275 -0.004786 173.052811" a="-83.052811" />
    <group name="Land_Mil_Tower_Small" pos="7918.434082 342.639648 14658.367188" rpy="0.002555 0.039482 -86.296692" a="176.296677" />
    <group name="Land_Mil_Tower_Small" pos="7939.082031 325.633240 14509.102539" rpy="-0.000000 0.000000 177.123810" a="-87.123817" />
    <group name="Land_Mil_Tower_Small" pos="7971.737305 342.589081 14616.348633" rpy="-0.019772 -0.000625 178.188675" a="-88.188675" />
    <group name="Land_Mil_Tower_Small" pos="7940.144043 363.048553 14803.253906" rpy="-0.000000 0.000000 35.060516" a="54.939476" />
    <group name="Land_Mil_Tower_Small" pos="8021.827148 326.378265 14517.349609" rpy="-0.000000 0.000000 174.199234" a="-84.199242" />
    <group name="Land_Mil_Tower_Small" pos="7982.034668 359.700592 14762.802734" rpy="-0.000000 0.000000 3.491943" a="86.508049" />
    <group name="Land_Mil_Tower_Small" pos="8069.214355 323.161377 14505.775391" rpy="-0.000000 0.000000 -168.632675" a="-101.367302" />
    <group name="Land_Mil_Tower_Small" pos="8070.290039 358.348022 14758.846680" rpy="-0.000000 0.000000 16.863123" a="73.136871" />
    <group name="Land_Mil_Tower_Small" pos="8151.593262 342.479309 14650.297852" rpy="-0.000000 0.000000 82.755196" a="7.244799" />
    <group name="Land_Mil_Tower_Small" pos="8126.684082 353.508759 14728.613281" rpy="-0.000000 0.000000 41.397167" a="48.602833" />
    <group name="Land_Mil_Tower_Small" pos="8167.135254 319.449615 14502.641602" rpy="-0.000000 0.000000 130.512848" a="-40.512852" />
    <group name="Land_Mil_Tower_Small" pos="11002.508789 223.832367 13380.983398" rpy="-0.000000 0.000000 104.266838" a="-14.266847" />
	
	<!--end of mapgrouppos.xml small guard tower xml snippet-->

Save your edited mapgrouppos.xml and re-upload if necessary.

Restart your community server and loot should start to appear on the watchtowers.

Please note that on local servers you may have to delelete your storage_1 folder to reset your server to see changes.

Also please note that we are adding many more potential loot placements for Military Clothes, Weapons & Explosives, so it may be worth considering
increasing their numbers slightly to compensate.

Thanks, Rob.