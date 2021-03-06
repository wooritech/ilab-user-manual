# 리포트 작성시 텍스트 상자를 틀에 맞게 일괄로 수정하기

이미 제작된 리포트를 상황에 따라 수정하시다보면 변수가 들어가는 텍스트칸이 틀어지는 경우가 있습니다.  이때, 수정을 하실때 칸의 높이와 넓이를 정수값으로 잡아주는 설정이 꺼져있게 되면 텍스트칸이 다른 칸들과 잘 맞지 않고 침범하게 되거나 부족하게 됩니다. 

또, 마우스로 늘리는 작업을 하더라도 정수가 아니기때문에 일일이 좌측의 OBJECT Inspector\(세부내용\) 탭에서 높이를 설정해줘야 하는 불편함이 있습니다. 

![&#xD2C0;&#xC758; &#xAC04;&#xACA9;&#xC774; &#xC81C;&#xB300;&#xB85C; &#xB9DE;&#xB294; &#xC54A;&#xB294; &#xACBD;&#xC6B0;](../.gitbook/assets/1.png)

위 그림과 같은 경우 정수값이 맞지 않아 마우스로 사용자께서 셀의 크기를 조정하시더라도 다른 셀과 크기가 맞지 않습니다.  이럴때 맞추고자 하는 셀들을 ctrl, shift + 클릭을 사용하셔서 모두 선택합니다.

![&#xD2C0;&#xC5B4;&#xC9C4; &#xC140;&#xB4E4;&#xC744; &#xBAA8;&#xB450; &#xC815;&#xC218;&#xAC12;&#xC73C;&#xB85C; &#xB9DE;&#xCDB0;&#xC8FC;&#xB294; &#xACFC;&#xC815;](../.gitbook/assets/16%20%285%29.png)

그 다음 상단의 정수로 변환하여주는 버튼을 클릭하시면 꼬여있던 셀의 크기\(0.47이나 0.63와 같은\)를

정수값으로 변환하여 줍니다.  

{% hint style="danger" %}
정수변환 버튼을 사용하셔도 모든 셀들을 같은 크기로 변환시켜주지는 않습니다.
{% endhint %}

 마지막으로 정수값으로 변환된 각 셀들을 한번만 클릭한뒤 테두리에 커서를 두고 크기를 조절해주시면     됩니다.

![&#xAC01; &#xC140;&#xB4E4;&#xC744; &#xC815;&#xC218;&#xB85C; &#xACE0;&#xC815;&#xC2DC;&#xCF1C;&#xC8FC;&#xB294; &#xAE30;&#xB2A5;](../.gitbook/assets/17%20%285%29.png)

{% hint style="info" %}
위와 같이 설정하신다음 리포트작업을 진행하시면 정수값을 나중에 다시 설정해주는 번거로움 없이 작업을 진행하실 수 있습니다.
{% endhint %}

{% hint style="success" %}
위와 같이 설정하셨더라도 좌측의 object inspector에서 정수값이 아니게 직접 크기를 변환시 정수값 설정이 안되고 그에 맞춰 크기가 늘어나게 되니 참고하시기 바랍니다. 
{% endhint %}

