# Optimization of the Sixth-Type Nonlinear Muskingum Model Incorporating Lateral Flow (NL6-LF)

This repository contains the implementation of the sixth-type nonlinear Muskingum flood routing model with lateral flow (NL6-LF). The model aims to improve the accuracy of flood routing by explicitly incorporating lateral inflows into the storage equation.

Case Studies:

The function Objfun.m is written in a general form.
Lines 18–20 of the Objfun.m file correspond to the input data (dt, I, and Q) of the selected case study.

For example, in the current version, lines 18–20 are defined for the seventh case study (Chenggou and Lingqing River flood dataset):
% Seventh case study: Chenggou and Lingqing river flood dataset

dt=1;

I=[261;389;462;505;525;543;556;567;577;583;587;595;597;597;589;556;538;516;486;505;477;429;379;320;263;220;182;167;152];

Q=[228;300;382;444;490;513;528;543;553;564;573;581;588;594;592;584;566;550;520;504;483;461;420;368;318;271;234;193;178]';

To test other case studies, replace lines 18–20 with the following definitions:
% First case study: Wilson 
dt=6;
I=[22;23;35;71;103;111;109;100;86;71;59;47;39;32;28;24;22;21;20;19;19;18];
Q=[22;21;21;26;34;44;55;66;75;82;85;84;80;73;64;54;44;36;30;25;22;19]';


% Second case study: Wye River
dt=1;
I=[154;150;219;182;182;192;165;150;128;168;260;471;717;1092;1145;600;365;277;277;187;161;143;126;115;102;93;88;82;76;73;70;67;63;59];
Q=[102;140;169;190;209;218;210;194;172;149;136;228;303;366;456;615;830;969;665;519;444;321;208;176;148;125;114;106;97;89;81;76;71;66]';


% Third case study: Viessman and Lewis 
dt=1;
I=[166.2;263.6;365.3;580.5;594.7;662.6;920.3;1568.8;1775.5;1489.5;1223.3;713.6;645.6;1166.7;1427.2;1282.8;1098.7;764.6;458.7;351.1;288.8;228.8;170.2;143];
Q=[118.4;197.4;214.1;402.1;518.2;523.9;603.1;829.7;1124.2;1379;1509.3;1379;1050.6;1013.7;1013.7;1013.7;1209.1;1248.8;1002.4;713.6;464.4;325.6;265.6;222.6]';


% Fourth case study: dataset of Sütçüler flood
dt=1;
I=[7.53;9.06;28;79.8;64.3;38.2;41.4;41.3;33.8;32;29;35;63.1;110;170;216;131;101;65;62.4;53.8;36.3;29.6;25;21.3;19.6;18;17.3;17;16];
Q=[7;8;23;25;75;60;40;41;41;32;30;34;35;60;105;160;206;128;97;61;60;50;33;27;23;19;18;17;17;17]';


% Fifth case study: dataset of the Karun River flood
dt=2;
I=[380;430;445;460;475;490;505;520;540;560;595;630;770;910;995;1080;1095;1110;1125;1140;1170;1200;1250;1300;1255;1210;1180;1150;1125;1100;1070;1040;995;950;885;820;800;780;760;740;730;720;720;720;730;740;750];
Q=[380;383.5;387;393;399;408.5;418;436;455;470;485;496;507;523.5;540;558;576;702.5;829;938.5;1048;1061.5;1075;1082;1089;1103;1117;1149.5;1182;1153;1124;1099.5;1075;1061.5;1048;1011;974;935;897;872.5;848;829.5;811;797;783;774.5;766]';


% Sixth case study: Brutsaert’s dataset
dt=1;
I=[139;172;250;438;736;1077;1622;2090;2294;2247;2090;1622;1271;1015;844;711;627;549;488;433;388;343;313;283;266;249;236;224;213;201;192;182];
Q=[139;139;124;220;342;542;805;1270;1684;1973;2169;2090;1895;1622;1333;1077;891;759;651;558;496;434;396;350;319;296;265;235;220;204;197;189]';


% Seventh case study: Chenggou and Lingqing river flood dataset (already shown above)


% Eighth case study: Ramirez’s dataset
dt=1;
I=[85;93;137;208;320;442;546;630;678;691;675;634;571;477;390;329;247;184;134;108;90];
Q=[85;85;91;114;159;233;324;420;509;578;623;642;635;603;546;479;413;341;274;215;170]';



