---
ms.openlocfilehash: ad624a665dbe8e989ea05acc20213809e515e6ac
ms.sourcegitcommit: 0be8a279af6d8a43e03141e349d3efd5d35f8767
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/18/2019
ms.locfileid: "59804579"
---
### <a name="incorrect-code-generation-when-passing-and-comparing-uint16-values"></a>UInt16 값 전달 및 비교 시 잘못된 코드 생성

|   |   |
|---|---|
|세부 정보|.NET Framework 4.7에서 변경된 내용으로 인해 .NET Framework 4.7에서 실행되는 애플리케이션의 JIT 컴파일러에서 생성된 코드가 두 개의 <code>T:System.UInt16</code> 값을 잘못 비교하는 경우가 있습니다. 자세한 내용은 GitHub.com에서 [문제 #11508: ushort 인수를 전달하고 비교할 때 자동 불량 codegen](https://github.com/dotnet/coreclr/issues/11508)을 참조하세요.|
|제안 해결 방법|.NET Framework 4.7에서 16비트 부호 없는 값을 비교할 때 문제가 발생하는 경우 .NET Framework 4.7.1로 업그레이드합니다.|
|범위|Microsoft Edge|
|버전|4.7|
|형식|런타임|
