Vogliamo creare uno spazio virtuale in stile social network dove gli utenti possano condividere le proprie esperienze. Ogni utente può creare dei post, al quale può aggiungere media come foto e video. Gli altri utenti possono interagire con il post esprimendo il loro gradimento attraverso un semplice "mi piace".

## Table: Users

- id: BIGINT AI UNIQUE PK NOT NULL
- name: VARCHAR(20) NOT NULL 
- surname: VARCHAR(20) NOT NULL
- password: VARCHAR(20) NOT NULL
- date_of_birth: DATE NOT NULL 
- email: VARCHAR(30) NOT NULL UNIQUE
- telefono: INT NULL 

## Table: Posts

- id: BIGINT AI UNIQUE PK NOT NULL
- user_id: FK
- title: VARCHAR(30) NOT NULL
- date_post: DATETIME DEFAULT NULL
- description: TEXT NOT NULL
- tags: VARCHAR(30) NULL

## Table: Medias

- id BIGINT AI UNIQUE PK NOT NULL
- photo NULL
- video NULL

## Table: media_post

- media_id
- post_id 

## Table: Likes

- id BIGINT AI UNIQUE PK NOT NULL
- user_id: FK
- post_id: FK

## Table: Comments

- id BIGINT AI UNIQUE PK NOT NULL
- post_id: FK
- user_id: FK
- text: TEXT NOT NULL
- date_comment: DATETIME NULL DEFAULT

