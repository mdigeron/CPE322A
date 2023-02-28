# Lab 9 - YANG
## CPE-322-A

**Install pyang and PlantUML**

![Screenshot (656)](https://user-images.githubusercontent.com/97755080/221863040-0c300de8-86f2-4f5e-bb02-d77edfd3daa7.png)

**copy ~/iot/lesson9/intrusiondetection.yang to ~/demo**

![Screenshot (657)](https://user-images.githubusercontent.com/97755080/221863424-537d7f7d-8d95-4e0a-9499-f2692bacb562.png)

```
module intrusiondetection {

 namespace "http://netconfcentral.org/ns/intrusiondetection";

 prefix "intrusion";

 description
  "YANG module for Intrusion Detection IoT system";

 revision 2014-07-15 {
  description "Intrusion Detection System";
 }

 grouping room {
  leaf doorsensorID {
   type string;
   description
    "ID of door sensor in the room";
  }
  leaf motionsensorID {
   type string;
   description
    "ID of motion sensor in the room";
  }
 }

 container intrusiondetection {
  presence
   "Indicates the service is available";

  description
   "Top-level container for all system objects.";

  leaf systemID {
   type string;
   config false;
   mandatory true;
   description
   "ID of the system";
  }

  leaf systemLocation {
   type string;
   config false;
   mandatory true;
   description
   "The location of the system";
  }

  leaf systemStatus {
   type enumeration {
    enum up {
    value 1;
    description
     "This is powered up";
    }
    enum down {
    value 2;
    description
     "This is powered down";
    }
    enum armed {
    value 3;
    description
     "This is armed";
    }
    enum disarmed {
    value 4;
    description
     "This is disarmed";
    }
   }
   config false;
   mandatory true;
   description
   "This variable indicates the current state of
    the system.";
  }
    container sensors {
   uses room;
   config false;
  }
 }

 rpc arm-system {
  description
   "Arm the system";
 }

 rpc disarm-system {
  description
   "Disarm the system";
 }

 notification systemArmed {
  description
   "Indicates that system has been armed.";

  leaf armStatus {
   description
    "Indicates the system arming status";

   type enumeration {
    enum armed {
    description
     "The system was armed.";
    }

    enum disarmed {
    description
     "The system was disarmed.";
    }

    enum error {
    description
     "The system is broken.";
    }
   }
  }
 }
}
```

**Run pyang to generate intrusiondetection.yin and intrusiondetection.uml**

![Screenshot (660)](https://user-images.githubusercontent.com/97755080/221864055-2efe3486-b977-4b36-9533-ec7e13b265a2.png)

```
<?xml version="1.0" encoding="UTF-8"?>
<module name="intrusiondetection"
        xmlns="urn:ietf:params:xml:ns:yang:yin:1"
        xmlns:intrusion="http://netconfcentral.org/ns/intrusiondetection">
  <namespace uri="http://netconfcentral.org/ns/intrusiondetection"/>
  <prefix value="intrusion"/>
  <description>
    <text>YANG module for Intrusion Detection IoT system</text>
  </description>
  <revision date="2014-07-15">
    <description>
      <text>Intrusion Detection System</text>
    </description>
  </revision>
  <grouping name="room">
    <leaf name="doorsensorID">
      <type name="string"/>
      <description>
        <text>ID of door sensor in the room</text>
      </description>
    </leaf>
    <leaf name="motionsensorID">
      <type name="string"/>
      <description>
        <text>ID of motion sensor in the room</text>
      </description>
    </leaf>
  </grouping>
  <container name="intrusiondetection">
    <presence value="Indicates the service is available"/>
    <description>
      <text>Top-level container for all system objects.</text>
    </description>
    <leaf name="systemID">
      <type name="string"/>
      <config value="false"/>
      <mandatory value="true"/>
      <description>
        <text>ID of the system</text>
      </description>
    </leaf>
    <leaf name="systemLocation">
      <type name="string"/>
      <config value="false"/>
      <mandatory value="true"/>
      <description>
        <text>The location of the system</text>
      </description>
    </leaf>
    <leaf name="systemStatus">
      <type name="enumeration">
        <enum name="up">
          <value value="1"/>
          <description>
            <text>This is powered up</text>
          </description>
        </enum>
        <enum name="down">
          <value value="2"/>
          <description>
            <text>This is powered down</text>
          </description>
        </enum>
        <enum name="armed">
          <value value="3"/>
          <description>
            <text>This is armed</text>
          </description>
        </enum>
        <enum name="disarmed">
          <value value="4"/>
          <description>
            <text>This is disarmed</text>
          </description>
        </enum>
      </type>
      <config value="false"/>
      <mandatory value="true"/>
      <description>
        <text>This variable indicates the current state of
the system.</text>
      </description>
    </leaf>
    <container name="sensors">
      <uses name="room"/>
      <config value="false"/>
    </container>
  </container>
  <rpc name="arm-system">
    <description>
      <text>Arm the system</text>
    </description>
  </rpc>
  <rpc name="disarm-system">
    <description>
      <text>Disarm the system</text>
    </description>
  </rpc>
  <notification name="systemArmed">
    <description>
      <text>Indicates that system has been armed.</text>
    </description>
    <leaf name="armStatus">
      <description>
        <text>Indicates the system arming status</text>
      </description>
      <type name="enumeration">
        <enum name="armed">
          <description>
            <text>The system was armed.</text>
          </description>
        </enum>
        <enum name="disarmed">
          <description>
            <text>The system was disarmed.</text>
          </description>
        </enum>
        <enum name="error">
          <description>
            <text>The system is broken.</text>
          </description>
        </enum>
      </type>
    </leaf>
  </notification>
</module>
```

![Screenshot (661)](https://user-images.githubusercontent.com/97755080/221864537-8d6b1d2f-b581-4044-8f93-81b42ca99ae6.png)

**Run PlantUML to generate intrusiondetection.png**

![Screenshot (663)](https://user-images.githubusercontent.com/97755080/221864873-a8bb6692-7c32-418f-bede-9f21831fcee8.png)

![Screenshot (664)](https://user-images.githubusercontent.com/97755080/221865153-96e4a954-8a69-4ee5-a780-b2995bff94e1.png)
