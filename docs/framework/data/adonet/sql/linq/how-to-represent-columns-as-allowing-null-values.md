---
title: '방법: 열을 NULL 값을 허용하는 열로 표현'
ms.date: 03/30/2017
ms.assetid: ebb71a37-1f4c-4fa7-b2d2-d903f13c4af1
ms.openlocfilehash: ef8fa87963b91ef7140fbaefb657fc7904604b5b
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "61902917"
---
# <a name="how-to-represent-columns-as-allowing-null-values"></a>방법: 열을 NULL 값을 허용하는 열로 표현
사용 합니다 [!INCLUDE[vbtecdlinq](../../../../../../includes/vbtecdlinq-md.md)] <xref:System.Data.Linq.Mapping.ColumnAttribute.CanBeNull%2A> 속성에는 <xref:System.Data.Linq.Mapping.ColumnAttribute> 연결 된 데이터베이스 열에 null 값을 가질 수는 지정 하는 특성입니다.  
  
 코드 예는 <xref:System.Data.Linq.Mapping.ColumnAttribute.CanBeNull%2A>를 참조하세요.  
  
### <a name="to-designate-a-column-as-allowing-null-values"></a>열을 null 값을 허용하는 열로 지정하려면  
  
1. <xref:System.Data.Linq.Mapping.ColumnAttribute.CanBeNull%2A> 특성에 <xref:System.Data.Linq.Mapping.ColumnAttribute> 속성을 추가합니다.  
  
2. <xref:System.Data.Linq.Mapping.ColumnAttribute.CanBeNull%2A> 속성 값을 `true`로 설정합니다.  
  
## <a name="see-also"></a>참고자료

- [LINQ to SQL 개체 모델](../../../../../../docs/framework/data/adonet/sql/linq/the-linq-to-sql-object-model.md)
- [방법: 코드 편집기를 사용 하 여 엔터티 클래스 사용자 지정](../../../../../../docs/framework/data/adonet/sql/linq/how-to-customize-entity-classes-by-using-the-code-editor.md)
