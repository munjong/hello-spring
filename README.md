# hello-spring
# hello-spring
# hello-spring
# hello-spring
# hello-spring



컴포넌트 스캔 방식
@Component 어노테이션으로 스프링빈에 등록해주면
서버 올릴때 해당객체를 스프링 컨테이너에서 관리해줌
(@Controller, @Service, @Repository)
(싱글톤 패턴으로 관리)

@Autowired 어노테이션으로 스프링빈에 등록된 객체를 매핑해준다
Controller - Service - Repository 의 의존관계를 가지고 있으면
Controller 에서 필요한 Service 객체를,
Service 에서 필요한 Repository 객체를
스프링에서 주입해준다
(대부분 생성자에 등록)

컴포넌트 스캔 방식 대신에 자바코드로 직접 등록하는 방법
클래스에 @Configuration 어노테이션을 등록해주고
@Bean 으로 객체 등록
-> 이 방법의 장점은 인터페이스 구조로 되있는 클래스의 구현 클래스를 변경해야 할 경우
이 부분만 수정해주면 됨