## build 방법
```
  mkdir build
  cd build
  cmake ..
  make
```
build에 파일 생성됨
```
  cd test
  ./GildedRoseTextTests.exe
  ./GildedRoseUnitTests.exe
  ./GildedRoseApprovalTests.exe
  
  cd ../../test/
  ls -al
  approval 파일이 없으면 아래 2개의 파일이 생성됨
  GildedRoseApprovalTests.VerifyCombinations.approved.txt
  GildedRoseApprovalTests.VerifyCombinations.received.txt
  
  rm -f GildedRoseApprovalTests.VerifyCombinations.approved.txt
  mv GildedRoseApprovalTests.VerifyCombinations.received.txt GildedRoseApprovalTests.VerifyCombinations.approved.txt

  cd ../build/test
  ./GildedRoseApprovalTests.exe

```


