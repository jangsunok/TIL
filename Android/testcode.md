

## Android Test Code


- AndroidJUnitRunner : JUnit4 기반 Android test runner
- Espresso : UI 테스팅 프레임워크, 앱에서 추가한 UI기능 테스트에 적합
- UI Automator : UI 테스팅 프레임워크, cross-app UI 테스팅에 적합
- JUnit : Unit Testing Framework (필수)
- Mockito : Mock Object 구현을 도와주는 라이브러리
- Hamcrest : Test Class 에서 사용하는 assert()와 같은 Matcher를 확장한 Library



## Annotation
- @Before : @Test를 시작하기 전 사전에 진행해야 할 사전 정의에 해당됩니다. @Test가 시작되기 전 항상 호출되게 됩니다.(단위 테스트 포함)
- @After : @After은 모든 테스트가 종료되면 호출되게 됩니다. 메모리에서 resource를 release 할 수 있습니다.
- @Test : @Before가 완료되면 실제 코드 테스트를 진행하게 됩니다.
- @Rule : 해당 Test class에서 사용하게 될 ActivityTestRule과 ServiceTestRule에 대하여 정의하게 됩니다.
- @BeforeClass, @AfterClass : public static method로 정의하여야 하며, @Before, @After와 동일하게 한 번씩만 실행되게 됩니다.
- @Test(timeout=
- @RequiresDevice : 에뮬레이터를 사용하지 않고 기기만 사용할 수 있습니다.
- @SdkSupress : minSdkVersion을 지정할 수 있습니다.
- @SmallTest, @MediumTest, @LargeTest : 테스트 성격을 구분하여 테스트할 수 있습니



## Reference
https://flowarc.tistory.com/entry/Android-Studio-%EB%8B%A8%EC%9C%84%ED%85%8C%EC%8A%A4%ED%8A%B8Unit-Test-%ED%95%98%EA%B8%B0
http://jepark-diary.tistory.com/19
https://thdev.tech/androiddev/2016/05/04/Android-Test-Example/
