# Generation.SourceGenerator

이 프로젝트는 C# Source Generator 예제입니다.
특정 Attribute([TestPartial])가 붙은 클래스에 대해 partial 코드를 자동 생성합니다.

## 주요 파일
- `TestPartialAttribute.cs`: 예시 Attribute 정의
- `MyPartialGenerator.cs`: Source Generator 구현

# 빌드 및 분석기 참조 방법
Generation.SourceGenerator 를 먼저 빌드하고 빌드결과물 경로를 Sample.csproj 파일의 <your path> 부분을 지우고 삽입합니다.
```
<Project Sdk="Microsoft.NET.Sdk">
  <PropertyGroup>
    <OutputType>Exe</OutputType>
    <TargetFramework>net9.0</TargetFramework>
    <ImplicitUsings>enable</ImplicitUsings>
    <Nullable>enable</Nullable>
  </PropertyGroup>
  <ItemGroup>
    <Analyzer Include="<your path>" />
  </ItemGroup>
</Project>
```
Sample 프로젝트의 Foo 클래스 사용시 소스가 생성됩니다. 


