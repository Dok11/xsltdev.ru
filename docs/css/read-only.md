---
description: Псевдокласс read-only применяется к полям формы, у которых задан атрибут readonly
---

# :read-only

Псевдокласс **`:read-only`** применяется к полям формы, у которых задан атрибут `readonly`. Такое поле не может быть модифицировано, при этом оно получает фокус, а данные в таком поле можно выделить и скопировать.

??? info "Псевдоклассы"

    <div class="col3" markdown="1">

    - [:active](active.md)
    - [:any-link](any-link.md)
    - [:blank](blank.md)
    - [:checked](checked.md)
    - [:current()](current.md)
    - [:default](default.md)
    - [:defined](defined.md)
    - [:dir()](dir.md)
    - [:disabled](disabled.md)
    - [:empty](empty.md)
    - [:enabled](enabled.md)
    - [:first](first.md)
    - [:first-child](first-child.md)
    - [:first-of-type](first-of-type.md)
    - [:focus](focus.md)
    - [:focus-visible](focus-visible.md)
    - [:focus-within](focus-within.md)
    - [:fullscreen](fullscreen.md)
    - [:future](future.md)
    - [:has()](has.md)
    - :host
    - :host()
    - :host-context()
    - [:hover](hover.md)
    - [:indeterminate](indeterminate.md)
    - [:in-range](in-range.md)
    - [:invalid](invalid.md)
    - [:is()](is.md)
    - [:lang()](lang.md)
    - [:last-child](last-child.md)
    - [:last-of-type](last-of-type.md)
    - [:left](left-pseudo-class.md)
    - [:link](link.md)
    - :local-link
    - [:not()](not.md)
    - [:nth-child()](nth-child.md)
    - :nth-col()
    - [:nth-last-child()](nth-last-child.md)
    - :nth-last-col()
    - [:nth-last-of-type()](nth-last-of-type.md)
    - [:nth-of-type()](nth-of-type.md)
    - [:only-child](only-child.md)
    - [:only-of-type](only-of-type.md)
    - [:optional](optional.md)
    - [:out-of-range](out-of-range.md)
    - [:past](past.md)
    - [:placeholder-shown](placeholder-shown.md)
    - **:read-only**
    - [:read-write](read-write.md)
    - [:required](required.md)
    - :right
    - [:root](root.md)
    - [:scope](scope.md)
    - [:target](target.md)
    - :target-within
    - :user-invalid
    - [:valid](valid.md)
    - [:visited](visited.md)
    - [:where()](where.md)

    </div>

## Синтаксис

```css
input:-moz-read-only {
  background: #eee;
}
input:read-only {
  background: #eee;
}
```

## Спецификации

- [HTML Living Standard](https://html.spec.whatwg.org/multipage/semantics-other.html#selector-read-only)
- [HTML5](https://www.w3.org/TR/html50/disabled-elements.html#selector-read-only)
- [Selectors Level 4](https://drafts.csswg.org/selectors-4/#rw-pseudos)
- [CSS Basic User Interface Module Level 3](https://drafts.csswg.org/css-ui-3/#pseudo-ro-rw)

## Пример

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>:read-only</title>
    <style>
      input:read-only {
        opacity: 0.3; /* Полупрозрачность */
      }
    </style>
  </head>
  <body>
    <form action="handler.php">
      <p>
        <input
          type="text"
          name="comment"
          size="40"
          value="Введенный текст не может изменяться"
          readonly
        />
      </p>

      <p><input type="submit" value="Отправить" /></p>
    </form>
  </body>
</html>
```

## См. также

- [:read-write](read-write.md)

## Ссылки

- Псевдо-класс [:read-write](https://developer.mozilla.org/ru/docs/Web/CSS/:read-only) <sup><small>MDN (рус.)</small></sup>
