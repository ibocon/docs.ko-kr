---
title: '방법: WebRequest를 사용하여 사용자 지정 프로토콜 등록'
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
ms.assetid: 98ddbdb9-66b1-4080-92ad-51f5c447fcf8
ms.openlocfilehash: 5c9a81fc61a2272056ba34fa387fdafee6203824
ms.sourcegitcommit: 0be8a279af6d8a43e03141e349d3efd5d35f8767
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/18/2019
ms.locfileid: "59079502"
---
# <a name="how-to-register-a-custom-protocol-using-webrequest"></a>방법: WebRequest를 사용하여 사용자 지정 프로토콜 등록
이 예제에서는 다른 곳에서 정의된 프로토콜별 클래스를 등록하는 방법을 보여줍니다. 이 예제에서 `CustomWebRequestCreator`는 `CustomWebRequest` 개체를 반환하는 **Create** 메서드를 구현하는 사용자가 구현한 개체입니다. 코드 예제에서는 사용자 지정 프로토콜을 구현하는 `CustomWebRequest` 코드를 작성했다고 가정합니다.  
  
## <a name="example"></a>예제  
  
```csharp  
WebRequest.RegisterPrefix("custom", new CustomWebRequestCreator());  
WebRequest req = WebRequest.Create("custom://customHost.contoso.com/");  
```  
  
```vb  
WebRequest.RegisterPrefix("custom", New CustomWebRequestCreator())  
Dim req As WebRequest = WebRequest.Create("custom://customHost.contoso.com/")  
```  
  
## <a name="compiling-the-code"></a>코드 컴파일  
 이 예제에는 다음 사항이 필요합니다.  
  
 <xref:System.Net> 네임스페이스에 대한 참조.  
  
## <a name="see-also"></a>참고 항목

- [플러그형 프로토콜 프로그래밍](../../../docs/framework/network-programming/programming-pluggable-protocols.md)
