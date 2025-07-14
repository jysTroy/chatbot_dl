# Chatbot 기능 개요

## 개요
본 프로젝트는 사용자 질문에 대해 자연스러운 한국어 답변을 생성하는 GPT2 기반 챗봇 시스템입니다.
백엔드는 Spring Boot로 구성되어 있고, 모델 추론은 Python에서 실행되며 KoGPT2 (skt/kogpt2-base-v2)를 사용합니다.

## 주요 기능
- Spring Boot ↔ Python 연동 
- transformers: 사전학습된 KoGPT2 모델과 토크나이저를 로드합니다.
- tensorflow: KoGPT2의 TensorFlow 기반 버전을 실행합니다.
- sys, json, os: 시스템 인자 처리 및 JSON 출력, 경로 계산에 사용됩니다.
- skt/kogpt2-base-v2: SKT에서 공개한 한국어 GPT2 모델.
- from_pt=True: PyTorch 모델 가중치를 TensorFlow로 변환하여 로드합니다.
- bos_token, eos_token, pad_token을 명시적으로 지정해 한국어 처리 성능을 보완합니다.
