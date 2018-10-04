# AI의 블랙박스화' 막겠다··· 오픈소스로 알고리즘 공개 선언한 IBM

원문보기: 
http://www.ciokorea.com/news/39723?page=0,0#csidx8045ada96223492b647c0a90d4e97d1 

## 블랙박스 알고리즘
또한 이런 툴은 알고리즘 디자인의 블랙박스를 여는데 유용하다는 점이 입증될 수 있다.

TLS(Times Literary Supplement)에서 출판된 그의 저서 신들의 죽음(The Death of Gods)에서 칼 밀러는 이렇게 말했다. "알고리즘이 정말 단순한 것에서 터무니없이 복잡한 것으로 바뀌었다. 이전과는 달리 과업을 달성하고 문제를 해결할 수 있다. 실제로 헤아릴 수 없이 복잡한 세상을 인간보다 더 잘 다룰 수 있다. 하지만 그런 것이 가능하기 때문에 그 작동 방식이 터무니없어졌다."

이 저서에서 익명을 요구한 한 대형 기술기업의 연구원은 밀러에게 다음과 같이 말했다. "힘은 있지만 책임감은 없는 것이다. 힘이 너무 세고 책임은 너무 없다. 개념적으로 추상적인 힘이 아니다. 일상을 위한 진정한 힘이다. 물질적이면서도 문화적이고 금융적이다. 이런 메커니즘을 알아야 한다."

그 연구원이 밀러에게 설명한 현재 알고리즘의 문제는 기하급수적인 데이터와 컴퓨팅 능력의 성장으로 알고리즘 훈련을 위해 엄청난 데이터를 제공할 수 있지만 우리는 인간으로서 알고리즘이 결론에 도달하는 데 실제로 도움이 된 입력값이 무엇인지 정의하기가 어려워진 것이다. 하나의 블랙박스인 것이다.

해당 연구원은 "현실적으로 문제가 있을 때만 내부를 살펴본다. 그리고 실제로 무슨 일이 일어났는지 이해하는 것이 물리적으로 불가능하다"고 결론 내렸다. 그는 "알고리즘이 할 일을 하는 것처럼 보이고 사람들이 불평하지 않는다면 현실을 파악하기 위해 모든 지침과 추상화된 코드 계층을 실제로 살펴볼 유인이 크지 않은 것이 현실이다"고 덧붙였다.

핀터레스트(Pinterest)의 수석 과학자 겸 스탠포드대학교의 머신러닝 교수인 또 다른 연구원 주어 레스코벡은 밀러에게 "우리는 한 단계 발전하여 선입견 없이 알고리즘을 평가할 방법을 찾아야 한다. 우리는 그들의 결정을 해석하고 설명할 수 있어야 한다. 우리가 최적의 알고리즘을 원하는 것이 아니다. 우리는 전문가가 살펴보고 이상한 일이 일어나지 않고 있다고 말할 수 있을 만큼 단순한 것을 원한다. 우리는 이런 것들을 이해관계 결정 환경에서 사회적인 배치에 대비시킬 방법을 진지하게 생각해 보아야 한다. 일정 수준의 품질을 확보하기 위해서는 어떻게 디버깅(Debugging)해야 할까?"고 말했다.

대형 기술업체들이 최소한 점차 자체 알고리즘에 내재된 위험이 적절한 감독 없이 사회를 위협하고 있다는 점을 인식하고 블랙박스를 해소할 조처를 하고 있는 것으로 보인다. 

원문보기: 
http://www.ciokorea.com/news/39723?page=0,1#csidx16523709641ad56b457fd29488ecbb6 


# Watson APIs Java SDK

[![Build Status](https://travis-ci.org/watson-developer-cloud/java-sdk.svg?branch=master)](https://travis-ci.org/watson-developer-cloud/java-sdk)
[![Slack](https://wdc-slack-inviter.mybluemix.net/badge.svg)](https://wdc-slack-inviter.mybluemix.net)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.ibm.watson.developer_cloud/java-sdk/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.ibm.watson.developer_cloud/java-sdk)
[![CLA assistant](https://cla-assistant.io/readme/badge/watson-developer-cloud/java-sdk)](https://cla-assistant.io/watson-developer-cloud/java-sdk)

Java client library to use the [Watson APIs][wdc].

<details>
  <summary>Table of Contents</summary>
  
  * [Before you begin](#before-you-begin)
  * [Installation](#installation)
    * [Maven](#maven)
    * [Gradle](#gradle)
  * [Usage](#usage)
  * [Running in IBM Cloud](#running-in-ibm-cloud)
  * [Authentication](#authentication)
    * [IAM](#iam)
    * [Username and password](#username-and-password)
    * [API key](#api-key)
  * IBM Watson Services
    * [Assistant](assistant)
    * [Discovery](discovery)
    * [Language Translator](language-translator)
    * [Natural Language Classifier](natural-language-classifier)
    * [Natural Language Understanding](natural-language-understanding)
    * [Personality Insights](personality-insights)
    * [Speech to Text](speech-to-text)
    * [Text to Speech](text-to-speech)
    * [Tone Analyzer](tone-analyzer)
    * [Tradeoff Analytics](tradeoff-analytics)
    * [Visual Recognition](visual-recognition)
  * [Android](#android)
  * [Configuring the HTTP client](#configuring-the-http-client)
  * [Default headers](#default-headers)
  * [Sending request headers](#sending-request-headers)
  * [Parsing HTTP response info](#parsing-http-response-info)
  * [Specifying a service URL](#specifying-a-service-url)
  * [401 unauthorized error](#401-unauthorized-error)
  * [Changes for v4.0](#changes-for-v40)
  * [Debug](#debug)
  * [Eclipse and Intellij](#working-with-eclipse-and-intellij-idea)
  * [License](#license)
  * [Contributing](#contributing)

</details>

## Before you begin
* You need an [IBM Cloud][ibm-cloud-onboarding] account.

## Installation

##### Maven

All the services:

```xml
<dependency>
	<groupId>com.ibm.watson.developer_cloud</groupId>
	<artifactId>java-sdk</artifactId>
	<version>6.7.0</version>
</dependency>
```

Only Discovery:

```xml
<dependency>
	<groupId>com.ibm.watson.developer_cloud</groupId>
	<artifactId>discovery</artifactId>
	<version>6.7.0</version>
</dependency>
```

##### Gradle

All the services:

```gradle
'com.ibm.watson.developer_cloud:java-sdk:6.7.0'
```

Only Assistant:

```gradle
'com.ibm.watson.developer_cloud:assistant:6.7.0'
```

##### Development snapshots

Snapshots of the development version are available in [Sonatype's snapshots repository][sonatype_snapshots].

###### Gradle

Add repository to your project Gradle file

```gradle
allprojects {
    repositories {
        maven { url "https://oss.sonatype.org/content/repositories/snapshots" }
    }
}
```

And then reference the snapshot version on your app module gradle
Only Speech to Text:

```gradle
'com.ibm.watson.developer_cloud:speech-to-text:6.7.1-SNAPSHOT'
```

##### JAR

Download the jar with dependencies [here][jar].

Now, you are ready to see some [examples](https://github.com/watson-developer-cloud/java-sdk/tree/master/examples/src/main/java/com/ibm/watson/developer_cloud).

## Usage

The examples within each service assume that you already have service credentials. If not,
you will have to [create a service](#getting-credentials) in IBM Cloud.

If you are running your application in IBM Cloud (or other platforms based on Cloud Foundry), you don't need to specify the
credentials; the library will get them for you by looking at the [`VCAP_SERVICES`][vcap_services] environment variable.

## Running in IBM Cloud

When running in IBM Cloud (or other platforms based on Cloud Foundry), the library will automatically get the credentials from [`VCAP_SERVICES`][vcap_services].
If you have more than one plan, you can use `CredentialUtils` to get the service credentials for an specific plan.

## Authentication

Watson services are migrating to token-based Identity and Access Management (IAM) authentication.

- With some service instances, you authenticate to the API by using **[IAM](#iam)**.
- In other instances, you authenticate by providing the **[username and password](#username-and-password)** for the service instance.
- Visual Recognition uses a form of [API key](#api-key) only with instances created before May 23, 2018. Newer instances of Visual Recognition use [IAM](#iam).

**Note:** Previously, it was possible to authenticate using a token in a header called `X-Watson-Authorization-Token`. This method is deprecated. The token continues to work with Cloud Foundry services, but is not supported for services that use Identity and Access Management (IAM) authentication. See [here](#iam) for details.

### Getting credentials
To find out which authentication to use, view the service credentials. You find the service credentials for authentication the same way for all Watson services:

1.  Go to the IBM Cloud [Dashboard](https://console.bluemix.net/dashboard/apps?category=ai) page.
1.  Either click an existing Watson service instance or click [**Create resource > AI**](https://console.bluemix.net/catalog/?category=ai) and create a service instance.
1.  Copy the `url` and either `apikey` or `username` and `password`. Click **Show** if the credentials are masked.

In your code, you can use these values in the service constructor or with a method call after instantiating your service.

### IAM

Some services use token-based Identity and Access Management (IAM) authentication. IAM authentication uses a service API key to get an access token that is passed with the call. Access tokens are valid for approximately one hour and must be regenerated.

You supply either an IAM service **API key** or an **access token**:

- Use the API key to have the SDK manage the lifecycle of the access token. The SDK requests an access token, ensures that the access token is valid, and refreshes it if necessary.
- Use the access token if you want to manage the lifecycle yourself. For details, see [Authenticating with IAM tokens](https://console.bluemix.net/docs/services/watson/getting-started-iam.html). If you want to switch to API key, override your stored IAM credentials with an IAM API key. Then call the `setIamCredentials()` method again.


#### Supplying the IAM API key
```java
// in the constructor, letting the SDK manage the IAM token
IamOptions options = new IamOptions.Builder()
  .apiKey("<iam_api_key>")
  .url("<iam_url>") // optional - the default value is https://iam.bluemix.net/identity/token
  .build();
Discovery service = new Discovery("2017-11-07", options);
```

```java
// after instantiation, letting the SDK manage the IAM token
Discovery service = new Discovery("2017-11-07");
IamOptions options = new IamOptions.Builder()
  .apiKey("<iam_api_key>")
  .build();
service.setIamCredentials(options);
```

#### Supplying the access token
```java
// in the constructor, assuming control of managing IAM token
IamOptions options = new IamOptions.Builder()
  .accessToken("<access_token>")
  .build();
Discovery service = new Discovery("2017-11-07", options);
```

```java
// after instantiation, assuming control of managing IAM token
Discovery service = new Discovery("2017-11-07");
IamOptions options = new IamOptions.Builder()
  .accessToken("<access_token>")
  .build();
service.setIamCredentials(options);
```

### Username and password

```java
// in the constructor
Discovery service = new Discovery("2017-11-07", "<username>", "<password>");
```

```java
// after instantiation
Discovery service = new Discovery("2017-11-07");
service.setUsernameAndPassword("<username>", "<password>");
```

### API key

**Important**: This type of authentication works only with Visual Recognition instances created before May 23, 2018. Newer instances of Visual Recognition use [IAM](#iam).

```java
// in the constructor
VisualRecognition service = new VisualRecognition("2016-05-20", "<api_key>");
```

```java
// after instantiation
VisualRecognition service = new VisualRecognition("2016-05-20");
service.setApiKey("<api_key>");
```

## Android

The Android SDK utilizes the Java SDK while making some Android-specific additions. This repository can be found [here](https://github.com/watson-developer-cloud/android-sdk). It depends on [OkHttp][] and [gson][].

## Configuring the HTTP client

The HTTP client can be configured by using the `configureClient()` method on your service object, passing in an `HttpConfigOptions` object. Currently, the following options are supported:
- Disabling SSL verification (only do this if you really mean to!) ⚠️
- Using a proxy (more info here: [OkHTTPClient Proxy authentication how to?](https://stackoverflow.com/a/35567936/456564))

Here's an example of setting both of the above:

```java
Discovery service = new Discovery("2017-11-07");

// setting configuration options
HttpConfigOptions options = new HttpConfigOptions.Builder()
  .disableSslVerification(true)
  .proxy(new Proxy(Proxy.Type.HTTP, new InetSocketAddress("proxyHost", 8080)))
  .build();

service.configureClient(options);
```

## Sending request headers

Custom headers can be passed with any request. To do so, add the header to the `ServiceCall` object before executing the request. For example, this is what it looks like to send the header `Custom-Header` along with a call to the Watson Assistant service:

```java
WorkspaceCollection workspaces = service.listWorkspaces()
  .addHeader("Custom-Header", "custom_value")
  .execute();
```

## Parsing HTTP response info

The basic `execute()`, `enqueue()`, and `rx()` methods make HTTP requests to your Watson service and return models based on the requested endpoint. If you would like access to some HTTP response information along with the response model, you can use the more detailed versions of those three methods: `executeWithDetails()`, `enqueueWithDetails()`, and `rxWithDetails()`. To capture the responses, use the new `Response<T>` class, with `T` being the expected response model.

Here is an example of calling the Watson Assistant `listWorkspaces()` method and parsing its response model as well as the response headers:

```java
Response<WorkspaceCollection> response = service.listWorkspaces().executeWithDetails();

// getting result equivalent to execute()
WorkspaceCollection workspaces = response.getResult();

// getting returned HTTP headers
Headers responseHeaders = response.getHeaders();
```

Note that when using `enqueueWithDetails()`, you must also implement the new `ServiceCallbackWithDetails` interface. For example:

```java
service.listWorkspaces().enqueueWithDetails(new ServiceCallbackWithDetails<WorkspaceCollection>() {
  @Override
  public void onResponse(Response<WorkspaceCollection> response) {
    WorkspaceCollection workspaces = response.getResult();
    Headers responseHeaders = response.getHeaders();
  }

  @Override
  public void onFailure(Exception e) { }
});
```

## Default headers

Default headers can be specified at any time by using the `setDefaultHeaders(Map<String, String> headers)` method.

The example below sends the `X-Watson-Learning-Opt-Out` header in every request preventing Watson from using the payload to improve the service.

```java
PersonalityInsights service = new PersonalityInsights("2016-10-19");

Map<String, String> headers = new HashMap<String, String>();
headers.put(HttpHeaders.X_WATSON_LEARNING_OPT_OUT, "true");

service.setDefaultHeaders(headers);

// All the api calls from now on will send the default headers
```

## Specifying a service URL

You can set the correct API endpoint for your service calling `setEndPoint()`.

For example, if you have the Discovery service in Germany, the endpoint may be `https://gateway-fra.watsonplatform.net/discovery/api`.

You will need to call

```java
Discovery service = new Discovery("2017-11-07");
service.sentEndPoint("https://gateway-fra.watsonplatform.net/discovery/api")
```

## 401 unauthorized error

Make sure you are using the service credentials and not your IBM Cloud account/password.
Check the API endpoint, you may need to update the default using `setEndPoint()`.

## Changes for v4.0
Version 4.0 focuses on the move to programmatically-generated code for many of the services. See the [changelog](https://github.com/watson-developer-cloud/java-sdk/wiki/Changelog) for the details. This version also includes many breaking changes as a result of standardizing behavior across the new generated services. Full details on migration from previous versions can be found [here](https://github.com/watson-developer-cloud/java-sdk/wiki/Migration).

## Debug

HTTP requests can be logged by adding a `logging.properties` file to your classpath.

```none
handlers=java.util.logging.ConsoleHandler
java.util.logging.ConsoleHandler.level=FINE
java.util.logging.ConsoleHandler.formatter=java.util.logging.SimpleFormatter
java.util.logging.SimpleFormatter.format=%1$tb %1$td, %1$tY %1$tl:%1$tM:%1$tS %1$Tp %2$s %4$s: %5$s%n
.level=SEVERE
# HTTP Logging - Basic
com.ibm.watson.developer_cloud.util.HttpLogging.level=INFO
```

The configuration above will log only the URL and query parameters for each request.

For example:

```none
Mar 30, 2017 7:31:22 PM okhttp3.internal.platform.Platform log
INFO: --> POST https://gateway.watsonplatform.net/tradeoff-analytics/api/v1/dilemmas?generate_visualization=false http/1.1 (923-byte body)
Mar 30, 2017 7:31:22 PM okhttp3.internal.platform.Platform log
INFO: <-- 200 OK https://gateway.watsonplatform.net/tradeoff-analytics/api/v1/dilemmas?generate_visualization=false (104ms, unknown-length body)
Mar 30, 2017 7:31:23 PM okhttp3.internal.platform.Platform log
INFO: --> POST https://gateway.watsonplatform.net/tradeoff-analytics/api/v1/dilemmas?generate_visualization=true http/1.1 (12398-byte body)
Mar 30, 2017 7:31:35 PM okhttp3.internal.platform.Platform log
INFO: <-- 200 OK https://gateway.watsonplatform.net/tradeoff-analytics/api/v1/dilemmas?generate_visualization=true (12311ms, unknown-length body)
```

**Warning:** The logs generated by this logger when using the level `FINE` or `ALL` has the potential to leak sensitive information such as "Authorization" or "Cookie" headers and the contents of request and response bodies. This data should only be logged in a controlled way or in a non-production environment.

## Build + test

To build and test the project you can use [Gradle][] (version 1.x).

Gradle:

```sh
cd java-sdk
gradle jar  # build jar file (build/libs/watson-developer-cloud-6.7.0.jar)
gradle test # run tests
gradle check # performs quality checks on source files and generates reports
gradle testReport # run tests and generate the aggregated test report (build/reports/allTests)
gradle codeCoverageReport # run tests and generate the code coverage report (build/reports/jacoco)
```

## Working with Eclipse and Intellij IDEA

If you want to work on the code in an IDE instead of a text editor you can
easily create project files with gradle:

```sh
gradle idea     # Intellij IDEA
gradle eclipse  # Eclipse
```

## Open source @ IBM

Find more open source projects on the [IBM Github Page](http://ibm.github.io/)

## License

This library is licensed under Apache 2.0. Full license text is
available in [LICENSE](LICENSE).

## Contributing

See [CONTRIBUTING.md](.github/CONTRIBUTING.md).

## Code of conduct

See [CODE_OF_CONDUCT.md](.github/CODE_OF_CONDUCT.md).

### Other

If you are having difficulties using the APIs or you have a question about the IBM
Watson Services, please ask a question on
[dW Answers](https://developer.ibm.com/answers/questions/ask/?topics=watson)
or [Stack Overflow](http://stackoverflow.com/questions/ask?tags=ibm-watson).


[wdc]: https://www.ibm.com/watson/developer/
[ibm_cloud]: https://console.bluemix.net
[Gradle]: http://www.gradle.org/
[OkHttp]: http://square.github.io/okhttp/
[gson]: https://github.com/google/gson
[apache_maven]: http://maven.apache.org/
[sonatype_snapshots]: https://oss.sonatype.org/content/repositories/snapshots/com/ibm/watson/developer_cloud/
[vcap_services]: https://console.bluemix.net/docs/services/watson/getting-started-variables.html
[ibm-cloud-onboarding]: http://console.bluemix.net/registration?target=/developer/watson&cm_sp=WatsonPlatform-WatsonServices-_-OnPageNavLink-IBMWatson_SDKs-_-Java


[jar]: https://github.com/watson-developer-cloud/java-sdk/releases/download/java-sdk-6.7.0/java-sdk-6.7.0-jar-with-dependencies.jar
