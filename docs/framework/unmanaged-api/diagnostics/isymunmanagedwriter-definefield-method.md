---
title: ISymUnmanagedWriter::DefineField 메서드
ms.date: 03/30/2017
api_name:
- ISymUnmanagedWriter.DefineField
api_location:
- diasymreader.dll
api_type:
- COM
f1_keywords:
- ISymUnmanagedWriter::DefineField
helpviewer_keywords:
- ISymUnmanagedWriter::DefineField method [.NET Framework debugging]
- DefineField method, ISymUnmanagedWriter interface [.NET Framework debugging]
ms.assetid: c6a1f797-dbf4-40f5-ab99-d9b4bfb26148
topic_type:
- apiref
author: mairaw
ms.author: mairaw
ms.openlocfilehash: 5fd9798b3681d66e71d5703f4d16564b153da07b
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "61789632"
---
# <a name="isymunmanagedwriterdefinefield-method"></a>ISymUnmanagedWriter::DefineField 메서드
메서드를 단일 변수를 정의 합니다. 이 방법은 클래스의 특정 필드, 비트 필드 등에 사용 합니다.  
  
## <a name="syntax"></a>구문  
  
```  
HRESULT DefineField(  
    [in] mdTypeDef    parent,  
    [in] const WCHAR  *name,  
    [in] ULONG32      attributes,  
    [in] ULONG32      cSig,  
    [in, size_is(cSig)] unsigned char signature[],  
    [in] ULONG32      addrKind,  
    [in] ULONG32      addr1,  
    [in] ULONG32      addr2,  
    [in] ULONG32      addr3);  
```  
  
## <a name="parameters"></a>매개 변수  
 `parent`  
 [in] 메타 데이터 형식 또는 메서드 토큰입니다.  
  
 `name`  
 [in] 필드 이름입니다.  
  
 `attributes`  
 [in] 필드 특성입니다.  
  
 `cSig`  
 [in] `ULONG32` 문자 필드 시그니처를 포함 하는 데 필요한 버퍼 크기입니다.  
  
 `signature`  
 [in] 배열 필드 시그니처입니다.  
  
 `addrKind`  
 [in] 주소 유형입니다.  
  
 `addr1`  
 [in] 필드 사양의 첫 번째 주소입니다.  
  
 `addr2`  
 [in] 필드 사양의 두 번째 주소입니다.  
  
 `addr3`  
 [in] 필드 사양의 세 번째 주소입니다.  
  
## <a name="return-value"></a>반환 값  
 메서드가 성공 하면 s_ok이 고 그렇지 않으면 E_FAIL 또는 일부 다른 오류 코드입니다.  
  
## <a name="requirements"></a>요구 사항  
 **헤더:** CorSym.idl, CorSym.h  
  
## <a name="see-also"></a>참고자료

- [ISymUnmanagedWriter 인터페이스](../../../../docs/framework/unmanaged-api/diagnostics/isymunmanagedwriter-interface.md)
