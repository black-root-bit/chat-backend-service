# chat-backend-service
Real-time WebSocket chat backend — private messages, group rooms, MongoDB
# 💬 chat-backend-service

> WebSocket-based real-time chat backend — private messaging, group rooms, message history, typing indicators, read receipts.

[![Java](https://img.shields.io/badge/Java-17-ED8B00?style=flat-square&logo=openjdk)](https://openjdk.org/)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.2-6DB33F?style=flat-square&logo=springboot)](https://spring.io/projects/spring-boot)
[![WebSocket](https://img.shields.io/badge/WebSocket-STOMP-FF6B35?style=flat-square)](https://stomp.github.io/)
[![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat-square&logo=mongodb)](https://mongodb.com)

**Features:** Real-time messaging via WebSocket/STOMP · Private 1:1 chats · Group rooms with admin controls · Message history (MongoDB) · Typing indicators · Read receipts · File attachment support (AWS S3) · Online/offline presence · Push notification integration

**WebSocket Topics:**
```
/app/chat.private.{userId}     # Send private message
/app/chat.room.{roomId}        # Send to room
/topic/user.{userId}           # Receive private messages
/topic/room.{roomId}           # Receive room messages
/topic/presence                # Online status updates
```

**REST Endpoints:**
```
GET   /api/v1/messages/{userId}/history     # Message history
GET   /api/v1/rooms                         # List rooms
POST  /api/v1/rooms                         # Create room
POST  /api/v1/rooms/{id}/members            # Add member
```

**GitHub Topics:** `java` `spring-boot` `websocket` `chat` `stomp` `mongodb` `real-time` `messaging` `docker`
