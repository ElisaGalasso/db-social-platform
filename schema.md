Vogliamo creare uno spazio virtuale in stile social network dove gli utenti possano condividere le proprie esperienze. Ogni utente può creare dei post, al quale può aggiungere media come foto e video. Gli altri utenti possono interagire con il post esprimendo il loro gradimento attraverso un semplice "mi piace".

## Table: User

- id
- name
- surname
- password
- date_of_birth
- email
- telefono

## Table: Post

- id
- user_id
- name
- date_post
- description
- tags

## Table: Media

- id
- post_id
- photo
- video

## Table: Likes

- id
- user_id
- post_id

## Table: Comments

- id
- post_id
- text
- date_comment

