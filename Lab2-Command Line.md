# CPE-322-A Lab 2 Command Line

## commands done on Windows Terminal

**hostname**

**env**

![Screenshot (520)](https://user-images.githubusercontent.com/97755080/216795667-ce039f8d-ba68-43a2-86bd-bb50c9b3817d.png)


**ps**

**pwd**

**git clone**

**cd iot**

**ls**

**cd**

**df**

**mkdir demo**

**cd demo**

![Screenshot (521)](https://user-images.githubusercontent.com/97755080/216795721-052ddddc-b8a1-4674-98b0-063983a3e541.png)


**nano file**

**cat file**

**cp file file1**

**mv file file2**

**rm file2**

![Screenshot (522)](https://user-images.githubusercontent.com/97755080/216795843-cd6ea4e8-c923-4723-b8af-5beeea75c52c.png)


**clear**

![Screenshot (523)](https://user-images.githubusercontent.com/97755080/216795846-f7215316-1324-4c49-b94c-e029ded399ea.png)


**man uname(WSL 2 Terminal)**

![Screenshot (528)](https://user-images.githubusercontent.com/97755080/216796862-872c3d9b-e3bc-4ef1-91e0-16578904dfd4.png)


![Screenshot (529)](https://user-images.githubusercontent.com/97755080/216796864-393ec6da-0530-4453-b5ec-d3c0f69e7616.png)



**uname -a(WSL 2 Terminal)**


![Screenshot (530)](https://user-images.githubusercontent.com/97755080/216796868-397fc883-a4ce-4832-a6dc-3865a31d6f4e.png)



**ipconfig(windows)**

![Screenshot (525)](https://user-images.githubusercontent.com/97755080/216795955-bbb75ba0-029b-4a45-aa51-fd0dce2ebbeb.png)


![Screenshot (526)](https://user-images.githubusercontent.com/97755080/216795960-2f1afdde-8c4c-420c-9b54-2934ee75201e.png)



**ping localhost**

![Screenshot (527)](https://user-images.githubusercontent.com/97755080/216796179-9e8223f2-9c2d-4198-8c9c-4e223968dee1.png)


**netstat (changed local addresses)**

```
C:\Users\Marc D\Downloads\iot\demo>netstat

Active Connections

  Proto  Local Address          Foreign Address        State
  TCP    xx.xx.x.x:49421        52.159.126.152:https   ESTABLISHED
  TCP    xx.xx.x.x:50111        13.107.21.200:https    CLOSE_WAIT
  TCP    xx.xx.x.x:50112        52.96.165.210:https    CLOSE_WAIT
  TCP    xx.xx.x.x:50113        bingforbusiness:https  CLOSE_WAIT
  TCP    xx.xx.x.x:50114        52.96.165.210:https    CLOSE_WAIT
  TCP    xx.xx.x.x:50115        a-0001:https           CLOSE_WAIT
  TCP    xx.xx.x.x:50116        52.182.143.211:https   CLOSE_WAIT
  TCP    xx.xx.x.x:50118        13.107.18.254:https    CLOSE_WAIT
  TCP    xx.xx.x.x:50119        13.107.238.41:https    CLOSE_WAIT
  TCP    xx.xx.x.x:50120        152.199.24.163:https   CLOSE_WAIT
  TCP    xx.xx.x.x:50121        204.79.197.222:https   CLOSE_WAIT
  TCP    xx.xx.x.x:51871        172.16.0.37:7474       ESTABLISHED
  TCP    xx.xx.x.x:53630        ec2-54-68-184-133:https  CLOSE_WAIT
  TCP    xx.xx.x.x:55458        64:domain              TIME_WAIT
  TCP    xx.xx.x.x:55464        162-254-192-74:27031   ESTABLISHED
  TCP    xx.xx.x.x:55471        a23-213-26-216:https   ESTABLISHED
  TCP    xx.xx.x.x:55472        a23-213-26-216:https   ESTABLISHED
  TCP    xx.xx.x.x:55473        a23-213-26-216:https   ESTABLISHED
  TCP    xx.xx.x.x:55474        a184-28-164-117:https  CLOSE_WAIT
  TCP    xx.xx.x.x:55475        a184-28-164-117:https  ESTABLISHED
  TCP    xx.xx.x.x:55477        ec2-52-88-138-244:https  ESTABLISHED
  TCP    xx.xx.x.x:55478        lb-140-82-113-4-iad:https  ESTABLISHED
  TCP    xx.xx.x.x:55479        s3-1-w:https           CLOSE_WAIT
  TCP    xx.xx.x.x:58902        52.96.97.162:https     CLOSE_WAIT
  TCP    xx.xx.x.x:60952        ec2-52-73-3-247:https  CLOSE_WAIT
  TCP    xx.xx.x.x:60955        ec2-52-73-3-247:https  CLOSE_WAIT
  TCP    xx.xx.x.x:61344        162.159.135.234:https  ESTABLISHED
  TCP    xx.xx.x.x:61347        dns9:https             ESTABLISHED
  TCP    xx.xx.x.x:61348        ww-in-f95:https        ESTABLISHED
  TCP    xx.xx.x.x:61349        ww-in-f95:https        ESTABLISHED
  TCP    xx.xx.x.x:61350        wv-in-f94:https        ESTABLISHED
  TCP    xx.xx.x.x:61352        lb-140-82-114-26-iad:https  ESTABLISHED
  TCP    xx.xx.x.x:61354        a23-7-43-2:https       ESTABLISHED
  TCP    xx.xx.x.x:61356        bh-in-f139:https       ESTABLISHED
  TCP    xx.xx.x.x:61359        52.96.28.178:https     ESTABLISHED
  TCP    xxx.x.x.x:4369         kubernetes:49746       ESTABLISHED
  TCP    xxx.x.x.x:4369         kubernetes:55460       TIME_WAIT
  TCP    xxx.x.x.x:4369         kubernetes:61345       TIME_WAIT
  TCP    xxx.x.x.x:9010         kubernetes:50061       ESTABLISHED
  TCP    xxx.x.x.x:9010         kubernetes:50078       ESTABLISHED
  TCP    xxx.x.x.x:9100         kubernetes:50068       ESTABLISHED
  TCP    xxx.x.x.x:27060        kubernetes:60747       ESTABLISHED
  TCP    xxx.x.x.x:49674        kubernetes:49675       ESTABLISHED
  TCP    xxx.x.x.x:49675        kubernetes:49674       ESTABLISHED
  TCP    xxx.x.x.x:49676        kubernetes:61900       ESTABLISHED
  TCP    xxx.x.x.x:49677        kubernetes:49678       ESTABLISHED
  TCP    xxx.x.x.x:49678        kubernetes:49677       ESTABLISHED
  TCP    xxx.x.x.x:49679        kubernetes:61900       ESTABLISHED
  TCP    xxx.x.x.x:49682        kubernetes:49815       ESTABLISHED
  TCP    xxx.x.x.x:49683        kubernetes:49684       ESTABLISHED
  TCP    xxx.x.x.x:49684        kubernetes:49683       ESTABLISHED
  TCP    xxx.x.x.x:49700        kubernetes:49701       ESTABLISHED
  TCP    xxx.x.x.x:49701        kubernetes:49700       ESTABLISHED
  TCP    xxx.x.x.x:49702        kubernetes:49721       ESTABLISHED
  TCP    xxx.x.x.x:49702        kubernetes:49723       ESTABLISHED
  TCP    xxx.x.x.x:49702        kubernetes:49724       ESTABLISHED
  TCP    xxx.x.x.x:49702        kubernetes:49725       ESTABLISHED
  TCP    xxx.x.x.x:49702        kubernetes:49730       ESTABLISHED
  TCP    xxx.x.x.x:49702        kubernetes:49733       ESTABLISHED
  TCP    xxx.x.x.x:49702        kubernetes:49737       ESTABLISHED
  TCP    xxx.x.x.x:49702        kubernetes:49804       ESTABLISHED
  TCP    xxx.x.x.x:49706        kubernetes:49707       ESTABLISHED
  TCP    xxx.x.x.x:49707        kubernetes:49706       ESTABLISHED
  TCP    xxx.x.x.x:49708        kubernetes:61900       ESTABLISHED
  TCP    xxx.x.x.x:49709        kubernetes:49710       ESTABLISHED
  TCP    xxx.x.x.x:49710        kubernetes:49709       ESTABLISHED
  TCP    xxx.x.x.x:49712        kubernetes:49842       ESTABLISHED
  TCP    xxx.x.x.x:49714        kubernetes:49715       ESTABLISHED
  TCP    xxx.x.x.x:49715        kubernetes:49714       ESTABLISHED
  TCP    xxx.x.x.x:49716        kubernetes:49717       ESTABLISHED
  TCP    xxx.x.x.x:49717        kubernetes:49716       ESTABLISHED
  TCP    xxx.x.x.x:49721        kubernetes:49702       ESTABLISHED
  TCP    xxx.x.x.x:49723        kubernetes:49702       ESTABLISHED
  TCP    xxx.x.x.x:49724        kubernetes:49702       ESTABLISHED
  TCP    xxx.x.x.x:49725        kubernetes:49702       ESTABLISHED
  TCP    xxx.x.x.x:49730        kubernetes:49702       ESTABLISHED
  TCP    xxx.x.x.x:49733        kubernetes:49702       ESTABLISHED
  TCP    xxx.x.x.x:49737        kubernetes:49702       ESTABLISHED
  TCP    xxx.x.x.x:49739        kubernetes:49740       ESTABLISHED
  TCP    xxx.x.x.x:49740        kubernetes:49739       ESTABLISHED
  TCP    xxx.x.x.x:49741        kubernetes:61900       ESTABLISHED
  TCP    xxx.x.x.x:49742        kubernetes:49743       ESTABLISHED
  TCP    xxx.x.x.x:49743        kubernetes:49742       ESTABLISHED
  TCP    xxx.x.x.x:49746        kubernetes:4369        ESTABLISHED
  TCP    xxx.x.x.x:49762        kubernetes:49763       ESTABLISHED
  TCP    xxx.x.x.x:49763        kubernetes:49762       ESTABLISHED
  TCP    xxx.x.x.x:49765        kubernetes:49766       ESTABLISHED
  TCP    xxx.x.x.x:49766        kubernetes:49765       ESTABLISHED
  TCP    xxx.x.x.x:49804        kubernetes:49702       ESTABLISHED
  TCP    xxx.x.x.x:49813        kubernetes:49814       ESTABLISHED
  TCP    xxx.x.x.x:49814        kubernetes:49813       ESTABLISHED
  TCP    xxx.x.x.x:49815        kubernetes:49682       ESTABLISHED
  TCP    xxx.x.x.x:49816        kubernetes:49817       ESTABLISHED
  TCP    xxx.x.x.x:49817        kubernetes:49816       ESTABLISHED
  TCP    xxx.x.x.x:49842        kubernetes:49712       ESTABLISHED
  TCP    xxx.x.x.x:49844        kubernetes:49845       ESTABLISHED
  TCP    xxx.x.x.x:49845        kubernetes:49844       ESTABLISHED
  TCP    xxx.x.x.x:49856        kubernetes:49857       ESTABLISHED
  TCP    xxx.x.x.x:49857        kubernetes:49856       ESTABLISHED
  TCP    xxx.x.x.x:50061        kubernetes:9010        ESTABLISHED
  TCP    xxx.x.x.x:50068        kubernetes:9100        ESTABLISHED
  TCP    xxx.x.x.x:50078        kubernetes:9010        ESTABLISHED
  TCP    xxx.x.x.x:60747        kubernetes:27060       ESTABLISHED
  TCP    xxx.x.x.x:60780        kubernetes:60781       ESTABLISHED
  TCP    xxx.x.x.x:60781        kubernetes:60780       ESTABLISHED
  TCP    xxx.x.x.x:60782        kubernetes:60783       ESTABLISHED
  TCP    xxx.x.x.x:60783        kubernetes:60782       ESTABLISHED
  TCP    xxx.x.x.x:61900        kubernetes:49676       ESTABLISHED
  TCP    xxx.x.x.x:61900        kubernetes:49679       ESTABLISHED
  TCP    xxx.x.x.x:61900        kubernetes:49708       ESTABLISHED
  TCP    xxx.x.x.x:61900        kubernetes:49741       ESTABLISHED
  TCP    [::1]:49670            DESKTOP-1PVTB6G:49671  ESTABLISHED
  TCP    [::1]:49671            DESKTOP-1PVTB6G:49670  ESTABLISHED
  TCP    [::1]:49672            DESKTOP-1PVTB6G:49673  ESTABLISHED
  TCP    [::1]:49673            DESKTOP-1PVTB6G:49672  ESTABLISHED
  TCP    [::1]:49680            DESKTOP-1PVTB6G:49681  ESTABLISHED
  TCP    [::1]:49681            DESKTOP-1PVTB6G:49680  ESTABLISHED
  TCP    [::1]:49686            DESKTOP-1PVTB6G:49687  ESTABLISHED
  TCP    [::1]:49687            DESKTOP-1PVTB6G:49686  ESTABLISHED
```

