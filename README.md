## Вопросы на собеседовании фронтенд разработчика React.js

**JavaScript**:
<details>
<summary>Типы данных</summary>
<div>
<ul>
<details>
<summary>Примитивные</summary>
<ul>
<li><b>«string»</b>: строки текста, например, "Hello, world!".</li>
<li><b>«number»</b>: числовые значения, как целые, так и дробные, например, 42 или 3.14.</li>
<li><b>«boolean»</b>: логические значения true или false.</li>
<li><b>«null»</b>: специальное значение, которое представляет отсутствие какого-либо значения.</li>
<li><b>«undefined»</b>: значение переменной, которая была объявлена, но не была инициализирована.</li>
<li><b>«symbol»</b>: уникальный и неизменяемый идентификатор, используется для создания уникальных ключей объектов.</li>
<li><b>«bigint»</b>: тип данных для представления целых чисел произвольной длины, например, 9007199254740991n.</li>
<br>
</ul>
</details>
<details>
<summary>Объектные</summary>
<ul>
<li><b>«object»</b>: коллекция свойств и методов, которая может включать объекты, массивы, функции и другие структуры данных.</li>
</ul>
</details>
</ul>
</div>
</details>
<details>
<summary>Цикл событий <b>(Event Loop)</b></summary>
<p><b>Event Loop</b> управляет выполнением кода, обработкой событий и выполнением асинхронных операций в JavaScript. Он следит за тем, чтобы задачи в очереди были выполнены после завершения текущего стека вызовов. Если в очереди есть задачи (например, асинхронные функции или обработчики событий), Event Loop добавляет их в стек вызовов для выполнения.</p>
</details>
<details>
<summary>Замыкание</summary>
<p>Замыкание возникает, когда функция запоминает переменные из своего лексического окружения, даже если она вызывается за пределами этой области видимости. Это позволяет функции получить доступ к переменным, которые существовали в момент её создания, что делает замыкания мощным инструментом для работы с состоянием и конфигурацией.</p>
</details>
<details>
<summary>Прототип объекта</summary>
<p>В JavaScript объекты могут наследовать свойства и методы от других объектов через прототипы. Если объект не имеет искомого свойства или метода, JavaScript будет искать его в прототипе этого объекта. Это механизм, позволяющий использовать наследование и переиспользование кода.</p>
</details>
<details>
<summary>Ключевое слово <b>«this»</b></summary>
<p><b>«this»</b> ссылается на текущий контекст выполнения функции. Контекст может меняться в зависимости от того, как была вызвана функция. Например, в методе объекта this будет ссылаться на объект, а в функции, вызванной в глобальной области, this будет ссылаться на глобальный объект (в браузере — на window).</p>
</details>
<details>
<summary>Методы <b>«call()»</b>, <b>«apply()»</b> и <b>«bind()»</b></summary>
<p>Эти методы используются для управления контекстом this в функциях:</p>
<ul>
<li><b>«call()»</b>: вызывает функцию с указанным контекстом this и передает аргументы по одному.</li>
<li><b>«apply()»</b>: аналогичен call(), но аргументы передаются в виде массива.</li>
<li><b>«bind()»</b>: возвращает новую функцию с фиксированным значением this, которую можно вызвать позже.</li>
</ul>
</details>
<details>
<summary><b>«Promise»</b> (Промис)</summary>
<p>Промисы позволяют работать с асинхронными операциями в JavaScript, избегая вложенности колбэков. Промис может быть в одном из трёх состояний:</p>
<ul>
<li><b>«pending»</b> (ожидание) — начальное состояние.</li>
<li><b>«fulfilled»</b> (выполнен) — операция завершена успешно.</li>
<li><b>«rejected»</b> (отклонён) — операция завершена с ошибкой.</li>
</ul>
</details>
<details>
<summary>Статический метод класса <b>(static)</b></summary>
<p>Методы, помеченные как static, могут быть вызваны непосредственно на классе, а не на его экземплярах. Они обычно используются для создания утилитарных функций, связанных с классом, но не с конкретным экземпляром.</p>
</details>
<details>
<summary><b>«Set»</b>, <b>«Map»</b>, <b>«WeakSet»</b>, <b>«WeakMap»</b></summary>
<ul>
<li><b>«Set»</b>: структура данных для хранения уникальных значений. Множество не допускает повторяющихся элементов.</li>
<li><b>«Map»</b>: структура данных, позволяющая хранить пары ключ-значение, где ключи могут быть любого типа.</li>
<li><b>«WeakSet»</b>: похож на Set, но хранит только объекты и позволяет сборщику мусора удалять неиспользуемые объекты.</li>
<li><b>«WeakMap»</b>: аналогичен Map, но ключами могут быть только объекты, и ссылки на них не предотвращают сборку мусора.</li>
</ul>
</details>

**React**:
<details>
<summary>Методы жизненного цикла компонента</summary>
<p>Классовые компоненты в React имеют методы, которые позволяют выполнять код на разных этапах жизненного цикла компонента:</p>
<ul>
<li><b>«componentDidMount»</b>: вызывается после того, как компонент был вставлен в DOM.</li>
<li><b>«componentDidUpdate»</b>: вызывается после обновления компонента.</li>
<li><b>«componentWillUnmount»</b>: вызывается перед удалением компонента из DOM.</li>
</ul>
</details>
<details>
<summary>Context в React</summary>
<p>Context предоставляет способ передавать данные (например, тему, язык) через дерево компонентов без необходимости передавать пропсы вручную на каждом уровне.</p>
</details>
<details>
<summary>Виртуальный <b>DOM</b></summary>
<p>Виртуальный <b>DOM</b> — это легковесное представление реального DOM. При изменении состояния компонента React сначала обновляет виртуальный DOM, затем вычисляет минимальные изменения и применяет их в реальном DOM, что позволяет избежать лишних обновлений и повышает производительность.</p>
</details>
<details>
<summary>Атрибут <b>«key»</b></summary>
<p><b>«key»</b> используется для уникальной идентификации элементов в списке. Это помогает React эффективно обновлять интерфейс, зная, какие элементы были изменены, добавлены или удалены.</p>
</details>
<details>
<summary>Пропc <b>«children»</b></summary>
<p><b>«children»</b> — это специальный пропс, который позволяет передавать вложенные элементы внутрь компонента. Используется, когда нужно отобразить произвольное количество дочерних элементов внутри компонента.</p>
</details>
<details>
<summary>Управляемые и не управляемые компоненты</summary>
<ul>
<li>Управляемые компоненты имеют свое состояние, контролируемое через React state, и изменение состояния компонента приводит к его перерисовке.</li>
<li>Не управляемые компоненты управляют своим состоянием самостоятельно, часто с использованием рефов для доступа к DOM-элементам напрямую.</li>
</ul>
</details>
<details>
<summary>PureComponent</summary>
<p>PureComponent — это компонент, который автоматически выполняет поверхностное сравнение пропсов и состояния для оптимизации производительности, предотвращая ненужные перерисовки.</p>
</details>
<details>
<summary>Компонент высшего порядка (HOC)</summary>
<p>HOC — это функция, которая принимает компонент и возвращает новый компонент с добавленным функционалом. Это шаблон для повторного использования кода в компонентах.</p>
</details>
<details>
<summary>Хуки в React:</summary>
<details>
<summary>useState</summary>
<ul>
<li><b>Назначение</b>: Управление состоянием в функциональных компонентах.</li>
<li><b>Принцип работы</b>: Возвращает массив из двух элементов: текущего состояния и функции для его обновления. При вызове функции обновления состояние обновляется, и компонент перерисовывается.</li>
</ul>
</details>
<details>
<summary>useEffect</summary>
<ul>
<li><b>Назначение</b>: Выполнение побочных эффектов, таких как запросы к API, изменение заголовков документа, установка подписок и др.</li>
<li><b>Принцип работы</b>: Принимает функцию эффекта и массив зависимостей. Эффект выполняется после рендера компонента и при изменении зависимостей. Также можно вернуть функцию очистки, которая выполнится перед следующим эффектом или при размонтировании компонента.</li>
</ul>
</details>
<details>
<summary>useContext</summary>
<ul>
<li><b>Назначение</b>: Доступ к значению контекста, созданного с помощью React.createContext.</li>
<li><b>Принцип работы</b>: Позволяет компоненту подписываться на изменения контекста и получать его значение, не передавая его через пропсы.</li>
</ul>
</details>
<details>
<summary>useReducer</summary>
<ul>
<li><b>Назначение</b>: Управление состоянием с использованием редюсера, что полезно для более сложной логики состояния.</li>
<li><b>Принцип работы</b>: Принимает редюсер (функцию для обработки действий) и начальное состояние. Возвращает текущее состояние и функцию dispatch, которая отправляет действия для обновления состояния.</li>
</ul>
</details>
<details>
<summary>useMemo</summary>
<ul>
<li><b>Назначение</b>: Оптимизация производительности путем кэширования вычисленных значений.</li>
<li><b>Принцип работы</b>: Принимает функцию, вычисляющую значение, и массив зависимостей. Возвращает кэшированное значение, если зависимости не изменились, что предотвращает повторные вычисления.</li>
</ul>
</details>
<details>
<summary>useCallback</summary>
<ul>
<li><b>Назначение</b>: Оптимизация производительности путем кэширования функций.</li>
<li><b>Принцип работы</b>: Принимает функцию и массив зависимостей. Возвращает кэшированную функцию, которая пересоздается только при изменении зависимостей. Это помогает избежать ненужных рендеров дочерних компонентов, которые зависят от этой функции.</li>
</ul>
</details>
<details>
<summary>useRef</summary>
<ul>
<li><b>Назначение</b>: Сохранение мутабельных значений и доступ к DOM-элементам.</li>
<li><b>Принцип работы</b>: Возвращает объект с текущим свойством (current). Этот объект сохраняется между рендерами и может использоваться для хранения любых значений или ссылок на DOM-элементы.</li>
</ul>
</details>
<details>
<summary>useImperativeHandle</summary>
<ul>
<li><b>Назначение</b>: Настройка значений, возвращаемых ref, для родительских компонентов.</li>
<li><b>Принцип работы</b>: Используется совместно с forwardRef. Позволяет настраивать и контролировать, что именно будет доступно родительским компонентам через ref.</li>
</ul>
</details>
</details>

<details>
<summary></summary>
</details>

<details>
<summary></summary>
</details>

<details>
<summary></summary>
</details>

<details>
<summary></summary>
</details>

<details>
<summary></summary>
</details>

<details>
<summary></summary>
</details>

<details>
<summary></summary>
</details>

<details>
<summary></summary>
</details>

