* `selectedServices`, `selectedServiceId`, `quantity` использовались без `useState`
* мутация `selectedServices`
* `totalPrice` всегда будет 0, так как selectedServices всегда пустой на момент рендера
* select и input без `setState`
* `selectedServices.find(item => item.service === service)` сравнение нужно через `id`
* `const index = selectedServices.indexOf(item)` - искать надежнее по `id`
* нет валидации `quantity` и `selectedServiceId`
* React импортирован, но не используется