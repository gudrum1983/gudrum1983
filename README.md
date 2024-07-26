<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    summary {
      cursor: pointer;
      list-style: none;
    }
    summary::-webkit-details-marker {
      display: none;
    }
    summary::before {
      content: "👉";
      display: inline-block;
      margin-right: 10px;
      transform: rotate(0deg);
      transition: transform 0.3s ease;
    }
    details[open] summary::before {
      transform: rotate(90deg);
    }
    details > div {
      overflow: hidden;
      transition: max-height 0.5s ease-out, opacity 0.5s ease-out;
      max-height: 0;
      opacity: 0;
    }
    details[open] > div {
      max-height: 500px; /* Задайте максимальную высоту содержимого */
      opacity: 1;
    }
  </style>
</head>
<body>
  <details>
    <summary> Разверните для просмотра краткой информации о проектах или перейдите в 📌 Pinned</summary>
    <div>
      <ol>
        <li>
          <p style="font-size: 14px; font-weight: 600">🚋 Путешествия по России</p>
          <ul style="padding-bottom: 10px">
            <li>Создала адаптивный интерфейс с использованием Flex, Grid и медиазапросов для обеспечения корректного отображения сайта на различных устройствах.</li>
            <li>Применяла методологию БЭМ для улучшения структуры и поддерживаемости кода.</li>
            <details>
              <summary style="margin: 10px 0">👉 Скриншоты сайта</summary>
              <div>
                <img src="images/traveling.png" style="height: 300px; border-radius: 10px; box-shadow: 0 0 5px; margin: 5px" alt="Хедер, главная картинка и заголовок">
                <img src="images/img_1.png" style="height: 300px; border-radius: 10px; box-shadow: 0 0 5px; margin: 5px" alt="Информационные статьи про памятные места">
                <img src="images/img.png" style="height: 300px; border-radius: 10px; box-shadow: 0 0 5px; margin: 5px" alt="Альбом с фото">
              </div>
            </details>
          </ul>
        </li>
        <li>
          <p style="font-size: 14px; font-weight: 600">📊 Визуализатор работы алгоритмов и структур данных</p>
          <ul style="padding-bottom: 10px">
            <li>Для реализации пошагового визуализатора работы алгоритмов и структур данных изучила и внедрила паттерн проектирования «Снимок» (Memento), что значительно повысило переиспользуемость кода.</li>
            <li>Проект включает тестирование с использованием Cypress, Jest и React Testing Library.</li>
          </ul>
        </li>
        <li>
          <p style="font-size: 14px; font-weight: 600">🍔👽 Космическая бургерная</p>
          <ul style="padding-bottom: 10px">
            <li>Разработала интерактивное веб-приложение для создания бургеров, управления профилем и отслеживания заказов в реальном времени с помощью WebSocket и REST API.</li>
            <li>Использовала Redux и Middleware для эффективного управления состоянием.</li>
            <li>Внедрила React Router для удобной навигации и работы с заказами, а также react-intersection-observer и Drag-and-drop для улучшения пользовательского опыта.</li>
          </ul>
        </li>
      </ol>
    </div>
  </details>
</body>
</html>
