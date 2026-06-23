# aiffel-gpt1-ir-coaching
# GPT-1 기반 IR 코칭 문장 생성 봇

AIFFEL Main Quest 프로젝트입니다.

## 프로젝트 목표

GPT-1 구조를 이해하고, IR 코칭 문장 데이터로 다음 토큰을 생성하는 소형 언어모델을 구현했습니다.

## 주요 구현 내용

* IR 코칭 합성 데이터셋 2,000개 제작
* Tokenizer, 정수 인코딩, Padding
* 입력 X와 정답 y를 한 칸 이동한 다음 토큰 예측
* Token Embedding + Position Embedding
* Masked Multi-Head Self-Attention
* Decoder-only GPT 모델 구현
* 입력 문장에 따른 IR 코칭 문장 생성

## 주요 파일

* `GPT-1.ipynb` : 전체 코드 및 실행 결과
* `ir_coaching_merged_2000.csv` : 학습 데이터셋
* `GPT1_IR_coaching_project.pptx` : 발표자료

## 한계와 개선 방향

현재 모델은 IR 관련 문장 생성에는 성공했지만, 사용자의 현재 IR 단계를 정확히 분류하지는 못했습니다.

다음 버전에서는 현재 단계, 부족 항목, 다음 행동, 코칭 질문을 라벨링하여 분류 모델과 생성 모델을 결합할 예정입니다.
