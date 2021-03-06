  - [Block Chain](#block-chain)

   * [종류](#종류)

   * [개발 과정](#개발-과정)

   * [이더리움](#이더리움)

      - [1세대 블록체인과 이더리움의 차이점](#1세대-블록체인과-이더리움의-차이점)

      - [Geth(Go-ethereum)](#geth-go-ethereum)

   * [Reference](#reference)


# Block-Chain

> 블록체인은 보안성이 높은 분산 데이터 저장기술의 한 형태이다.
>
> 관리 대상 데이터를 '블록'이라고 하는 소규모 데이터들이 P2P 방식을 기반으로 생성된 체인 형태의 연결고리 기반 분산 데이터 저장 환경에 저장하여 누구라도 임의로 수정할 수 없고 누구나 변경의 결과를 열람할 수 있는 분산 컴퓨팅 기술 기반의 원장 관리 기술이다.

### 탈중앙화

암호화폐의 노드는 부분 또는 전체의 블록체인을 가지고 있다. 이것이 페이팔과 같은 시스템에서 필요로 하는, 중앙 집중형 데이터베이스를 가지고 있을 필요가 없게 한다. 블록체인은 자체로 거래내역, 거래장부, 거래증서 역할을 수행한다. 

"지불인 갑이 00원을 수취인 을에게 보낸다" 형식의 거래는 소프트웨어 앱(ex. metamask)을 통해 블록체인 네트워크에 뿌려진다. 블록체인 네트워크의 노드들은 거래를 검증한 다음, 자신의 장부에 거래를 추가한다. 그리고 이 거래가 추가된 장부를 네트워크의 다른 노드들에 뿌린다.



## 종류

`공개 블록체인`: 접근 제한이 전혀 없는 블록체인

`비공개 블록체인`: 특정 권한이 부여된 비공개 블록체인

`하이브리드 블록체인`: 중앙식, 탈 중앙식 기능을 모두 갖춘 블록체인

## 개발 과정

블록체인의 첫 구현체 개발은 **비트코인**으로 시작되었고, 추가적으로 성능개선, 익명성 추가, 저장기능, 스마트 컨트랙트 기능이 개발되었다.



## 이더리움

화폐 기능에서 더 나아가 **블록체인 기술을 기반으로 스마트 컨트랙트 기능을 구현하기 위한 `분산 컴퓨팅 플랫폼`이자 운영체제**이다.

이더리움에서 스마트 계약을 처리하기 위한 가상 머신은 모든 형태의 알고리즘을 처리할 수 있는 튜링기계로서, 먼저 들어온 데이터를 우선적으로 처리하는 스택 구조를 가진다. EVM은 저수준의 기계에 가까운 바이트 코드만을 실행할 수 있기 때문에 고급 프로그래밍 언어를 실행하기 위해서는 바이트 코드로 컴파일 과정을 거쳐야 한다. 이 가상머신을 이용하기 위해서는 '가스'라는 대가를 지불해야한다. 이더리움 자체는 C++, 자바, 파이썬, Go 등 주요 프로그래밍 언어를 지원한다.

### 1세대 블록체인과 이더리움의 차이점

1. 암호해시 함수

   Ethash라는 ECCACK 기반의 해시 알고리즘을 개발해서 사용한다.

2. Modified Merkle Patricia Trie(MPT)

   MPT는 트랜잭션 데이터의 위변조 감지 및 스마트 컨트랙트 관련 상태 정보를 저장, 관리하기 위한 기술입니다. 상태정보는 key-value 형태로 저장됩니다.

3. 사용자 계정 기반 관리

   블록체인은 블록 기반으로 정보를 관리하는 반면, 이더리움은 사용자 기반으로 블록 관점으로 관리합니다.

### Geth, Go-ethereum

`Geth`는 이더리움 클라이언트 중 Go 언어로 개발된 버전이며, 현재 가장 많이 쓰이고 있는 이더리움 명령줄 도구입니다.

명령행 부속 명령 및 옵션, JSON-RPC 서버, 대화식 콘솔 세 가지 인터페이스를 제공합니다.



## Reference

https://ko.wikipedia.org/wiki/%EB%B8%94%EB%A1%9D%EC%B2%B4%EC%9D%B8

https://ko.wikipedia.org/wiki/%EC%9D%B4%EB%8D%94%EB%A6%AC%EC%9B%80

http://wiki.hash.kr/index.php/%EA%B2%8C%EC%8A%A4
