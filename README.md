# Velmie Client's headers requirements

---

**Version**: 

---

## Headers

* V-Client-Name
* V-Client-Platform
* V-Client-Device-Id
* V-Client-Version-Name
* V-Client-Version-Build
* V-Client-Version-Commit
* V-Client-Session-Id
* V-Client-Request-Id

---

### Example

```
V-Client-Name: App Name Mobile Flutter
V-Client-Platform: iOS 14.4
V-Client-Device-Id: 46317361-69bc-4475-a552-17d7f4cca8be
V-Client-Version-Name: 1.0.3
V-Client-Version-Build: 47
V-Client-Version-Commit: fd5064f
V-Client-Session-Id: 36a54006-71df-4234-8db3-d6ba02ed72d5
V-Client-Request-Id: fd4c197b-eb02-4568-a0ff-9f0e31284831
```

### Description

**V-Client-Name**: The name of the client. For example, it can be a `hybrid` or native mobile app, frontend app, package, etc.

**V-Client-Platform**: Usually it is a type of operational system, like iOS, Android, Mac, Windows, Linux, etc.

**V-Client-Device-Id**: A unique identifier of the device.

**V-Client-Version-Name**: A version of the software.

**V-Client-Version-Build**: The number of the build. Usually, it is started at 1 and increased by 1 with each build of the software.

**V-Client-Version-Commit**: The reference to a particular commit hash that is used to build the software.

**V-Client-Session-Id**: A unique identifier of the client's session. E.g.:

* For a library, it is generated each time after its initialization;
* For a mobile app it is generated each time when the app has started;
* For a frontend app it is generated each time  when the app has been loaded by a user via a browser;

**V-Client-Request-Id**: A unique identifier of the request to the server/backend. It should be re-generated every request, i.e. - be unique. It is used to trace the whole request path.

---
