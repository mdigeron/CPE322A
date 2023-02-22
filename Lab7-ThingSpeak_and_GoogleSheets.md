# Lab 7- ThingSpeak and Google Sheets
## CPE-322-A

**Sign up and log in MathWorks ThingSpeak**

Note: may have trouble loading sign in page if you have a [VPN](https://en.wikipedia.org/wiki/VPN_service) running.

**Run thingspeak_cpu_loop.py or thinkspeak_feed.py in a demo folder**

![Screenshot (629)](https://user-images.githubusercontent.com/97755080/220673873-56cfbcb0-f568-4d29-9178-b92e958de63d.png)

![Screenshot (630)](https://user-images.githubusercontent.com/97755080/220674121-939d33ef-8d68-4878-ab6c-74834ea13b58.png)

**Install gspread and oauth2client**

![Screenshot (619)](https://user-images.githubusercontent.com/97755080/220477973-990ca79a-5c81-4112-889f-fa286c84fcc3.png)

![Screenshot (620)](https://user-images.githubusercontent.com/97755080/220477987-9bf97067-26b1-492f-804a-a2e91fd11a6b.png)

**Log in the Google Cloud Platform Identity and Access Management, create a project cpudata, enable both Drive API and Sheets API, create and download service account JSON key file**

![Screenshot (621)](https://user-images.githubusercontent.com/97755080/220481998-c924c5fc-5583-48f6-a889-2d7aea619a85.png)

![Screenshot (622)](https://user-images.githubusercontent.com/97755080/220482018-577eab05-77d8-43bb-bd01-40688016151d.png)

![Screenshot (628)](https://user-images.githubusercontent.com/97755080/220482075-e430f769-b2a3-424c-8438-95432a5be420.png)

**Start a new Google sheet cpudata, share it with the client email in the JSON file, delete Rows 2 to 1000, and edit the header cells**

![Screenshot (623)](https://user-images.githubusercontent.com/97755080/220481810-2b6a9f7c-cd86-4cb1-850e-92fceca9d316.png)

![Screenshot (627)](https://user-images.githubusercontent.com/97755080/220481866-e9237016-cc42-4b42-8f3c-9e33bfeaca66.png)

**Run cpu_spreadsheet.py with the JSON key file in a demo folder**

![Screenshot (624)](https://user-images.githubusercontent.com/97755080/220481897-f2118cd9-0a21-4a51-9913-0933f87a26d2.png)

![Screenshot (625)](https://user-images.githubusercontent.com/97755080/220481906-1bace674-5cd8-41bd-8099-4cfb733142a9.png)

edited formating 
![Screenshot (626)](https://user-images.githubusercontent.com/97755080/220481933-0b2aa584-27ff-4fdf-9e52-b1e159f064c3.png)
