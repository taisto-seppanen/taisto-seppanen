### Hi there 👋 My name is Taisto

### Contacts:

- Telegram: [@taisto_seppanen](https://t.me/taisto_seppanen "@taisto_seppanen")
- E-mail: taistopetrseppanen@gmail.com

### Skills

- QA & Testing / HTML / CSS / JavaScript / Git / Vue.js / Nuxt.js / Bootstrap

### Code examples

    import firebase from "firebase/app";

    export async function setNewFilm(newfilm) {
      await firebase
        .database()
        .ref("films/")
        .set({ newfilm });
    }

    export async function getFilms() {
      let filmsArr = [];
      await firebase
        .database()
        .ref("films/")
        .get()
        .then(snapshot => {
          if (snapshot.exists()) {
            filmsArr = snapshot.val().newfilm;
          } else {
            console.warn("bad request");
          }
        });
      return filmsArr;
    }

### Experience

Now i'm working as QA engineer in [Roskavral company](https://roskvartal.ru/o-kompanii)

In 2021 i was complete advanced training courses of modern web development.
- Sipmle [snake game](https://taisto-seppanen.github.io/Snake/ "Snake Game")
- Trainee website for [cinema booking](https://cinimabooking.herokuapp.com/ "cinema booking") with admin page (/login) and database at Firebase
- Trainee website for [Louvre](https://rolling-scopes-school.github.io/taisto-seppanen-JSFEPRESCHOOL/museum/)
- Trainee website [Louvre](https://rolling-scopes-school.github.io/taisto-seppanen-JSFEPRESCHOOL/museum/)
- Trainee website [wildlife](https://rolling-scopes-school.github.io/taisto-seppanen-JSFE2021Q1/wildlife/)


### English

My english level is A2, but I can easily read documentation and technical literature.

<!--
**taisto-seppanen/taisto-seppanen** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
