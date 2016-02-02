# AndroidSocketClient
socket client 简易封装

## Import
[JitPack](https://jitpack.io/)

Add it in your project's build.gradle at the end of repositories:

```gradle
repositories {
  // ...
  maven { url "https://jitpack.io" }
}
```

Step 2. Add the dependency in the form

```gradle
dependencies {
  compile 'com.github.vilyever:AndroidSocketClient:1.1.0'
}
```

## Usage
```java

VDSocketClient socketClient = new VDSocketClient();
socketClient.registerDelegate(new VDSocketClient.VDSocketClientDelegate() {
    @Override
    public void didConnect(VDSocketClient client) {

    }

    @Override
    public void didDisconnect(VDSocketClient client) {

    }

    @Override
    public void didReceiveResponse(VDSocketClient client, String response) {

    }
});
socketClient.connect("192.168.1.1", 80);
```

## License
[Apache License Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.txt)

