# 성적서에 공란을 넣어 출력하는 방법

## Q

성적서를 출력할 때 A4용지 크기에 맞게 항목이 표기되고,

항목이 적을 경우 공란 또는 빈 공간을 넣어 출력하고 싶습니다.

어떻게 해야하나요?

\(아래 첨부 확인부탁드립니다.\)

![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/01공란이_없는_양식.1.png)

-&gt; 

![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/02잘못된_행계산.1.png)

## A

※ 아이랩 상단 메뉴 중 공통/코드관리 -&gt; 리포트관리2.0 메뉴가 보이지 않는 분이라면,  
관리자분께 요청하셔서 권한을 받으시거나 관리자분께 요청하여 작업을 진행 해 보시기 바랍니다.  
※ 성적서관리, 통합접수목록 등의 화면에 있는 목록에서 나오는 데이터는 리포트 양식에서  
MasterDataBand\(노란색 밴드\)와 연결이 되어집니다.

※ 아이랩 성적서는 현재 A4용지를 기준으로 양식 작업이 이루어지고 있습니다.  
따라서 A4용지의 규격인 297mm X 210mm \(세로 X 가로\)를 사용하고있습니다.

1. 공통/코드관리 -&gt; 리포트 관리2.0 화면으로 이동.  
2. 성적서 탭클릭  
3. 원하는 성적서를 선택 후 리포트 디자인 버튼클릭 또는 원하는 성적서를 더블 클릭.  
4. 리포트디자이너에서 MasterData1을 선택 후 ctrl + c -&gt; ctrl + v \(복사 후 붙여넣기\)  

   \(빈 공란이 데이터가 나오는 모양과 같아야 하기 때문입니다.\)  

   ![](../.gitbook/assets/03%20%2832%29.png)

   -&gt;

   ![](../.gitbook/assets/04-2%20%281%29.png)

5. 빈 공란으로 보여져야 하기 때문에, 데이터가 나올 수 있도록 연결 되어 있는 부분을 제거  

   \(MasterData2 에 속해 있는 모든 메모 개체를 선택 -&gt; 마우스 우측버튼 클릭 -&gt; Clear Contents 선택\)  

   ![](../.gitbook/assets/05%20%289%29.png)

   ![](../.gitbook/assets/06clearcontents%20%281%29.png)

6. 새로 만들어진 MasterDataBand를 선택 후 이름을 변경 MasterData2 -&gt; mdSpace  

   \(왼쪽에 있는 Properties 부분에 Name 속성을 변경해주면됩니다.\)  

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/07mdSpace1.png)

   -&gt; 

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/07mdSpace.png)

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/07mdSpace2.png)

   -&gt; 

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/07mdSpace3.png)

7. 페이지 여백 및 다른 밴드들의 영역크기 계산  

   아래 나오는 높이들을 계산기 또는 암산으로 계산해주세요.  

   \(MasterData1 과 mdSpace 의 높이는 제외 합니다.\)  

   공란의 높이 = \(A4용지의 전체 높이 - \(각밴드들의 Height의 합 + 페이지 상, 하단의 여백\)\)  

   ```text
             = 29.7 - (0.8 + 2.7 + 1.4 + (2 + 1))  
             = 21.8  
   ```

   공란의 행의 갯수 = 공란의 높이 / MasterData1의 높이  

   ```text
                    = 21.8 / 0.8  
                    = 27.25 (반올림이 가능 할 때는 반올림 하여 처리해주세요.)  
   ```

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/08ReportTitleHeight.png)

   -&gt; 

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/09ReportTitle.png)

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/10ColumnHeader.png)

   -&gt; 

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/11ColumnHeaderHeight.png)

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/12Pagefooter.png)

   -&gt; 

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/13PagefooterHeight.png)

   리포트 디자이너 왼쪽 상단 file -&gt; PageSettings 메뉴 클릭.  

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/14PageSettings.png)

8. Code 탭으로 이동.  

   begin 과 end. 사이에 아래 내용을 입력  

   if  &gt; 27 then  

   begin  

    mdSpace.RowCount := 27 - \( mod 27\);  

   end  

   else  

   begin  

    mdSpace.RowCount := 27 - ;  

   end;  

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/15코딩.png)

9. 리포트 디자이너 오른쪽 상단에 있는 파일저장 버튼클릭  

   ![](https://github.com/wooritech/ilab-user-manual/tree/ccd67ba3c673210c7b8ed25f93692c7b2dd1afa3/assets/faq/002-17/16파일저장.png)

10. 실제 접수된건을 해당 성저서 양식으로 출력하여 공란이 잘 생성되는지 확인.  
11. 공란설정이 잘 된다면, 다른 선생님들도 적용 될 수 있도록 리포트관리2.0 화면에서 해당 양식을 선택 후 업로드 버튼 클릭.  

위에 방법대로 해보시고 잘 안되시면 잘 안되는 부분을 서비스 요청으로 보내주시기 바랍니다.

