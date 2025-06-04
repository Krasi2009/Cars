# 🚗 Prolog Коли + GIF Визуализация

Това е уеб приложение, което използва **Prolog логика в браузъра** за извеждане на информация за **различни коли**, базирано на заявки като:

- `is_fast(X).`
- `is_suv(X).`
- `is_german(X).`

Ако бъде намерена съвпадаща кола, се показва **анимирано GIF изображение** с нея.

---

## 🔗 Линк към сайта (GitHub Pages)

👉 [https://твоето-потребителско-име.github.io/prolog-cars-site](https://твоето-потребителско-име.github.io/prolog-cars-site)

---

## ⚙️ Как работи

1. Зарежда се вградена база с коли, написана на Prolog.
2. Потребителят въвежда заявка в стил `is_suv(X).`
3. Ако има съвпадения, показва резултата и GIF картинка на съответната кола.

---

## 📄 Примерна Prolog база

```prolog
car(bmw_m3).
car(mercedes_glc).
car(audi_q7).
car(porsche_911).
car(toyota_supra).
car(ford_mustang).

is_suv(X) :- member(X, [mercedes_glc, audi_q7]).
is_fast(X) :- member(X, [bmw_m3, porsche_911, toyota_supra, ford_mustang]).
is_german(X) :- member(X, [bmw_m3, mercedes_glc, audi_q7, porsche_911]).
