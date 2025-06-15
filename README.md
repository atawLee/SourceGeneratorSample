# Generation.SourceGenerator

이 프로젝트는 C# Source Generator 예제입니다.
특정 Attribute([TestPartial])가 붙은 클래스에 대해 partial 코드를 자동 생성합니다.

## 주요 파일
- `MyPartialAttribute.cs`: 예시 Attribute 정의
- `MyPartialGenerator.cs`: Source Generator 구현

## 빌드 방법
```
dotnet build
```

## 참고
- Microsoft.CodeAnalysis.CSharp 패키지 사용
- .NET 6 이상 권장
