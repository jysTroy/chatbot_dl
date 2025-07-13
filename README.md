# Chatbot 기능 개요

## 개요
본 프로젝트는 사용자 질문에 대해 자연스러운 한국어 답변을 생성하는 GPT2 기반 챗봇 시스템입니다.
백엔드는 Spring Boot로 구성되어 있고, 모델 추론은 Python에서 실행되며 KoGPT2 (skt/kogpt2-base-v2)를 사용합니다.

## 주요 기능
- 사용자 질문을 받아 GPT2 기반 모델로 응답 생성
- 프론트엔드에서 실시간 채팅 UI 제공
- Spring Boot ↔ Python 연동 (서버 내 로컬 실행)
  
