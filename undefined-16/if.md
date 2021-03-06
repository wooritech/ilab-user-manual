# 시험법 계산식 if문 사용법

## Q

계산식에 있는 함수 중에 if 문은 어떻게 쓰는지 방법을 알려주셨으면 합니다.

## A

### if문 사용의 기본 모양

```csharp
if 조건1 then 
실행문1
실행문2
...
elseif 조건2 then
실행문
else // 조건1, 조건2 둘 다 아닐 때
실행문
end if
```

{% hint style="info" %}
* 5, 6번 라인의 경우 생략이 가능합니다.
* 실행문1, 실행문2 처럼 줄을 바꾸어가며 여러 개의 실행문을 넣을 수 있습니다. 
* 여러 개의 조건이 필요할 때는 elseif 라는 조건문을 추가하여 사용합니다.
{% endhint %}

{% tabs %}
{% tab title="예시1" %}
**V1** 변수 이름의 값이 10보다 크다면 최종 결과값을 **V1**로, 아니라면 최종 결과값을 **V2**의 값으로

{% code-tabs %}
{% code-tabs-item title="예시1" %}
```csharp
if V1 > 10 then
Result = V1
else
Result = V2
end if
```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% hint style="info" %}
여기서 `Result`란 [검사결과등록3.0](https://help.ilabs.co.kr/05/3053) 화면의 시험결과값을 의미합니다.
{% endhint %}
{% endtab %}

{% tab title="예시2" %}
**V1** 변수값이 30이상일 때 최종결과는 **V1**, 20이상일 때는 **V2**, 10이상일 때는 **V3**, 모두 아니라면 **V4** 값으로

{% code-tabs %}
{% code-tabs-item title="예시2" %}
```csharp
if V1 >= 30 then 
Result = V1 
elseif V1 >= 20 then 
Result = V2 
elseif V1 >= 10 then 
Result = V3 
else 
Result = V4 
end if
```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% hint style="info" %}
해당 예시는 `V1` 변수의 값이 입력될 경우 바로 계산이 진행되어 시험결과값이 입력됩니다.
{% endhint %}
{% endtab %}
{% endtabs %}

