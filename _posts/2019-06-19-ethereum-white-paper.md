---
-layout: post
-title: Ethereum White Paper
-date:  2019-06-19 11:43:00 +0900
-categories: blog
---

# 이더리움 백서 요약

이더리움 백서를 읽으면 요약한 내용이므로 잘못 요약된 내용이 있을 수 있으니 반드시 원문을 참고하시길 바랍니다.

- [이더리움 백서 한글판](https://github.com/ethereum/wiki/wiki/%5BKorean%5D-White-Paper)
- [이더리움 백서 영문판](https://github.com/ethereum/wiki/wiki/White-Paper)


## 차세대 스마트 컨트랙트와 탈중앙화된 어플리케이션 플랫폼

사토시 나카모트가 개발한(2008 ~ 2009년) 비트코인은 근본적인 혁신으로 묘사되어지고 있는데 이는 중앙화된 발행기관이나, 통제기관도 없는 디지털 자산의 첫번째 사례였기 때문이다. 하지만 비트코인 실험의 더 중요한 측면은 비트코인을 떠 받치고 있는 분산합의수단으로서의 블록체인 기술이다.

블록체인 기술의 활용
- [컬러드 코인(colored coins)](https://docs.google.com/document/d/1AnkP_cVZTCMLIzw4DvsW6M8Q2JC0lIzrTLuoWu2z1BE/edit)
- [스마트 자산(smart property)](https://en.bitcoin.it/wiki/Smart_Property)
- [네임코인(name coin)](https://namecoin.org/)
- [스마트 컨트랙트(smart contracts)](https://en.bitcoin.it/wiki/Contracts)
- 블록체인 기반 탈중앙화된 자율 조직(decentralized autonomous organizations, DAOs)

이더리움이 제공하려는 것은 완벽한 튜링완전(turing-complete) 프로그래밍 언어가 심어진 블록체인이다. 이 프로그래밍 언어는 코딩된 규칙에 따라 `어떤 상태` 를 다르게 변환시키는 기능이 포함된 `계약(contracts)` 을 유저들이 작성할 수 있게 한다. 이로써 다른 많은 애플리케이션을 쉽게 만들 수 있도록 도와줄 것이다.


## 비트코인과 기존 개념들에 대한 소개

분산화된 디지털 통화의 개념은 재산등록과 같은 대안 어플리케이션과 마찬가지로 지난 수십 년간 우리 주변에 있었다.

- 익명 e-cash 프로토콜(1980 ~ 90년대)
    - `Chaumian blinding` 으로 알려진 로우 레벨 알고리즘(cryptographic primitive)을 기반으로 개인정보를 강력하게 보호하는 화폐를 제공
    - 중앙집권적인 중개인에 의존 

- b-money(1998년)
    - 분산합의와 계산 퍼즐을 풀게하는 방식을 통해서 화폐를 발행하는 아이디어(최초 제안)
    - 분산합의의 실제 구현을 제시하지 못함

- Hall finney(2005년)
    - 재사용 가능한 작업 증명(reusable proofs of work)
    - b-money의 아이디어에 Adam Back의 계산 난이도 해시캐시 퍼즐(computationally difficult Hashcash puzzles)을 조합한 것

- 사토시 나카모토의 탈중앙화된 화폐(2009년)
    - 처음으로 사토시 나카모토에 의해 실제로 구현된 탈중앙화된 화폐
    - 공개키 암호방식을 통한 소유권 관리를 위해 사용되던 기존의 알고리즘 + 작업 증명(proof of work) 합의 알고리즘과 결합
