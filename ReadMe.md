// Запрашиваем и загружаем данные о товарах из файла shop.json.
Promise.resolve(shopData)
  
  // Параметр data — массив объектов-товаров (в каталоге их 9),
  .then(data => {
    // Находим фрагмент на странице shop.html, в который нужно добавить товары.
    document.querySelector("#node_for_insert").innerHTML = data
      .map(product => `
        <li>
          <img src="${product.img}" alt="${product.title}" onerror="this.onerror=null;this.src='./images/tennis_${product.id}.svg'">
          <h6>${product.title}</h6>
          <p class="margin_01rem">${product.description}. Цена ${product.price} р.</p>
          <input type="hidden" name="vendor_code" value="${product.vendor_code}">
          <p class="margin_01rem">Заказать <input type="number" name="amount" value="0" min="0"></p>
        </li>
      `)
    // Объединяем массив шаблонов и убираем запятые.
    .join("");
  })
  // Если загрузить файл или обработать данные не удалось, выводим ошибку в консоль.
  .catch(error => console.error("Не удалось загрузить каталог товаров:", error));