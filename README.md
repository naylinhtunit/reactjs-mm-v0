# reactjs-mm-v0
# React.js ကို လေ့လာရန်အတွက် အဆင့်များ
## 1. JavaScript Fundamentals
React ကို သုံးစွဲရန်အတွက် JavaScript ကို အခြေခံကောင်းစွာ နားလည်ထားရမည်။ လေ့လာသင့်သည့်အရာများမှာ-
* Variables (var, let, const)
* Functions
* Arrow Functions
* Objects and Arrays
* ES6+ Syntax (Destructuring, Spread Operator, etc.)
* Promises and Async/Await
## 2. Setting Up the Environment
* Node.js and npm (Node Package Manager) ကို install ပြုလုပ်ပါ။
* Create-React-App (CRA) ကို အသုံးပြု၍ React Project တစ်ခု ဖန်တီးပါ။
## 3. React Basics
* Introduction to React
* JSX (JavaScript XML)
* Components
  * Function Components
  * Class Components
* Props (Properties)
* State
* Event Handling
## 4. Advanced Concepts
* Component Lifecycle Methods (Class Components)
* Hooks (Function Components)
  * useState
  * useEffect
  * Custom Hooks
* Context API
* Refs
* Error Boundaries
## 5. Styling in React
* CSS Stylesheets
* Inline Styles
* CSS Modules
* Styled Components
* Sass with React
## 6. React Router
* React Router Basics
* Route, Link, NavLink
* Dynamic Routing
* Nested Routes
* Redirects and Navigation
## 7. State Management
* Lifting State Up
* Context API
* Redux
  * Actions, Reducers, Store
  * Middleware (Redux Thunk, Redux Saga)
## 8. Handling Forms
* Controlled Components
* Uncontrolled Components
* Form Validation
* Form Libraries (Formik, React Hook Form)
## 9. API Integration
* Fetch API
* Axios
* Handling Async Data in React
* Custom Hooks for Data Fetching
## 10. Performance Optimization
* Memoization
* React.memo
* useMemo and useCallback Hooks
* Lazy Loading
* Code Splitting
## 11. Testing
* Jest
* React Testing Library
* Unit Testing
* Integration Testing
## 12. Build and Deployment
* Building for Production
* Deployment Options (Netlify, Vercel, GitHub Pages)
* Continuous Integration and Deployment (CI/CD)
## 13. Additional Learning
* TypeScript with React
* Server-Side Rendering (SSR) with Next.js
* Static Site Generation (SSG) with Next.js
* Progressive Web Apps (PWAs)
* GraphQL with React (Apollo Client)
## 14. Project Development
* Start building small projects
* Todo App, Weather App, E-commerce Site
* Contribute to open-source projects
* Build a portfolio


React.js ကို အခြေခံမှစ၍ အသေးစိတ် ဖော်ပြပေးထားပါသည်။
## 1. JavaScript Fundamentals
React ကို အသုံးပြုရန် JavaScript ကို အခြေခံကောင်းစွာ နားလည်ထားရမည်။ လေ့လာသင့်သည့်အရာများမှာ-

Variables (var, let, const)
JavaScript တွင် variable များကို သတ်မှတ်ရန် var, let, const များကို အသုံးပြုသည်။ var သည် function scope ဖြစ်ပြီး let နှင့် const များသည် block scope ဖြစ်သည်။ React တွင် state များကို ကိုင်တွယ်ရာတွင် const နှင့် let ကို အများဆုံးအသုံးပြုသည်။

```
// var
var nameVar = 'John';
console.log(nameVar); // John

// let
let nameLet = 'Jane';
console.log(nameLet); // Jane

// const
const nameConst = 'Jake';
console.log(nameConst); // Jake

// Note: const variable cannot be reassigned
// nameConst = 'Jack'; // This will throw an error
```
* Functions
JavaScript တွင် function များကို လုပ်ဆောင်ချက်တစ်ခုစီအတွက် သုံးသည်။ React မှာ components များကို function အဖြစ်ရေးနိုင်သည်။

```
function greet(name) {
  return `Hello, ${name}!`;
}

console.log(greet('John')); // Hello, John!
```
* Arrow Functions
Arrow functions သည် function expressions ကို ရေးရန် အဆင်ပြေစေသည်။ React တွင် event handler များကို သတ်မှတ်ရာတွင် အများဆုံးအသုံးပြုသည်။

```
const greet = (name) => `Hello, ${name}!`;

console.log(greet('Jane')); // Hello, Jane!
```
* Objects and Arrays
JavaScript မှာ objects နှင့် arrays များကို data structures အဖြစ်အသုံးပြုသည်။ React မှာ props နှင့် state များကို object နှင့် array အဖြစ် handle ပြုလုပ်သည်။

```
const person = { name: 'John', age: 30 };
const numbers = [1, 2, 3, 4, 5];

console.log(person.name); // John
console.log(numbers[0]); // 1
```
* ES6+ Syntax (Destructuring, Spread Operator, etc.)
ES6+ မှာ destructuring, spread operator စသည်တို့ပါဝင်သည်။ React မှာ data ကို pass through props မှာ အဆင်ပြေစေသည်။

```
const { name, age } = person;
console.log(name); // John

const moreNumbers = [...numbers, 6, 7, 8];
console.log(moreNumbers); // [1, 2, 3, 4, 5, 6, 7, 8]
```
* Promises and Async/Await
Promises နှင့် async/await ကို asynchronous operations များအတွက် အသုံးပြုသည်။ React မှာ API call များကို handle ပြုလုပ်ရာတွင် အသုံးဝင်သည်။

```
const fetchData = async () => {
  try {
    const response = await fetch('https://jsonplaceholder.typicode.com/posts/1');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
};

fetchData();
```
## 2. Setting Up the Environment
React project တစ်ခုကို စတင်ရန်အတွက် environment ကိုပြင်ဆင်ရမည်။

* Node.js and npm Installation
Node.js ကို Node.js website မှာ download ပြုလုပ်ပြီး install ပါ။ Node.js နှင့်အတူ npm (Node Package Manager) လည်း ပါဝင်လာပါသည်။ npm သည် React libraries များကို install ပြုလုပ်ရန် အသုံးပြုသည်။

* Create-React-App (CRA)
Create-React-App ကို အသုံးပြု၍ React Project အသစ်တစ်ခုကို လွယ်ကူစွာ ဖန်တီးနိုင်ပါသည်။ CRA သည် React application များကို အလွယ်တကူ စတင်နိုင်ရန် အထောက်အကူဖြစ်စေသည်။

```
npx create-react-app my-app
cd my-app
npm start
```
## 3. React Basics
* Introduction to React
React သည် Facebook မှ ဖန်တီးခဲ့ပြီး, User Interfaces (UIs) များကို ဖန်တီးရန်အတွက် JavaScript library တစ်ခုဖြစ်သည်။ React ၏ အဓိကအယူအဆမှာ component-based architecture ဖြစ်ပြီး, reusable components များကို အသုံးပြုသည်။

* JSX (JavaScript XML)
JSX သည် React ၏ UI components များကို ဖန်တီးရာတွင်အသုံးပြုသော syntax ဖြစ်ပြီး, HTML နှင့် ဆင်တူသော syntax ဖြစ်သည်။ JSX သည် JavaScript ကို extend ပြုလုပ်ပြီး React DOM မှာ rendering ပြုလုပ်ရန် အဆင်ပြေစေသည်။

```
const element = <h1>Hello, world!</h1>;

// In React component
function App() {
  return element;
}

// Render the App component to the DOM
ReactDOM.render(<App />, document.getElementById('root'));
```
* Components
React ၏ အခြေခံအဆင့်မှာ Components ဖြစ်သည်။ Component တစ်ခုသည် UI ၏ သီးခြားအစိတ်အပိုင်းတစ်ခုကို ကိုယ်စားပြုသည်။

* Function Components
Function Components သည် JavaScript functions ဖြစ်ပြီး, props ကို parameter အဖြစ်လက်ခံပါသည်။ Function Components ကို ရေးရန် လွယ်ကူပြီး ရိုးရှင်းသည်။

```
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

// Usage
function App() {
  return <Welcome name="John" />;
}

ReactDOM.render(<App />, document.getElementById('root'));
```
* Class Components
Class Components သည် ES6 class ကို အသုံးပြု၍ ဖန်တီးသည်။ Class Components သည် state နှင့် lifecycle methods များကို ကိုင်တွယ်ရာတွင် အထူးအသုံးပြုသည်။

```
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}

// Usage
function App() {
  return <Welcome name="Jane" />;
}

ReactDOM.render(<App />, document.getElementById('root'));
```
* Props (Properties)
Props သည် React Components များအကြား data ပေးပို့ရန် အသုံးပြုသည်။ Parent component မှ Child component သို့ data ပေးပို့ရာတွင် props ကို အသုံးပြုသည်။

```
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

// Usage
function App() {
  return <Welcome name="Jake" />;
}

ReactDOM.render(<App />, document.getElementById('root'));
```
* State
State သည် Component ၏ internal state ကို ကိုယ်စားပြုသည်။ State ကို Class Component နှင့် Function Component (Hooks) များတွင် အသုံးပြုနိုင်သည်။

Class Component မှာ State ကို အသုံးပြုပုံ
Class Component တွင် state ကို constructor တွင် သတ်မှတ်ပြီး, this.setState ကို အသုံးပြု၍ update ပြုလုပ်သည်။

```
class Clock extends React.Component {
  constructor(props) {
    super(props);
    this.state = { date: new Date() };
  }

  componentDidMount() {
    this.timerID = setInterval(() => this.tick(), 1000);
  }

  componentWillUnmount() {
    clearInterval(this.timerID);
  }

  tick() {
    this.setState({ date: new Date() });
  }

  render() {
    return (
      <div>
        <h1>Hello, world!</h1>
        <h2>It is {this.state.date.toLocaleTimeString()}.</h2>
      </div>
    );
  }
}

ReactDOM.render(<Clock />, document.getElementById('root'));
```
* Function Component မှာ State ကို အသုံးပြုပုံ (Hooks)
Function Components တွင် useState Hook ကို အသုံးပြုပြီး state ကို သတ်မှတ်နိုင်သည်။ useEffect Hook ကို အသုံးပြုပြီး lifecycle methods များကို handle ပြုလုပ်သည်။

```
import React, { useState, useEffect } from 'react';

function Clock() {
  const [date, setDate] = useState(new Date());

  useEffect(() => {
    const timerID = setInterval(() => setDate(new Date()), 1000);

    return () => clearInterval(timerID);
  }, []);

  return (
    <div>
      <h1>Hello, world!</h1>
      <h2>It is {date.toLocaleTimeString()}.</h2>
    </div>
  );
}

ReactDOM.render(<Clock />, document.getElementById('root'));
```
* Event Handling
React တွင် event handler များကို သတ်မှတ်ရန် HTML event attributes ကို အသုံးပြုနိုင်သလို JavaScript functions များကိုလည်း အသုံးပြုနိုင်သည်။ Event handling သည် user interaction များကို handle ပြုလုပ်ရန် လိုအပ်သည်။

* Class Component တွင် Event Handling
```
import React from 'react';

class Button extends React.Component {
  handleClick() {
    alert('Button clicked!');
  }

  render() {
    return (
      <button onClick={this.handleClick}>Click Me</button>
    );
  }
}

ReactDOM.render(<Button />, document.getElementById('root'));
```
* Function Component တွင် Event Handling
```
import React from 'react';

function Button() {
  function handleClick() {
    alert('Button clicked!');
  }

  return (
    <button onClick={handleClick}>Click Me</button>
  );
}

ReactDOM.render(<Button />, document.getElementById('root'));
```
## 4. Advanced Concepts
* Component Lifecycle Methods (Class Components)
Class Components တွင် lifecycle methods များသည် component ၏ creation, updates, နှင့် destruction အဆင့်များကို handle လုပ်ရန် အသုံးပြုသည်။ အဓိက methods များမှာ-

  * componentDidMount(): Component သည် DOM ထဲသို့ render ပြုလုပ်ပြီးနောက် run ပါသည်။ API calls များ၊ timers များ စတင်ရန် အသုံးပြုသည်။
  * componentDidUpdate(prevProps, prevState): Component သည် re-render ပြုလုပ်ပြီးနောက် run ပါသည်။
  * componentWillUnmount(): Component ကို DOM မှ remove သည့်အခါ run ပါသည်။ Cleanup (e.g., timers, subscriptions) များကို ပြုလုပ်ရန် အသုံးပြုသည်။
```
class MyComponent extends React.Component {
  componentDidMount() {
    console.log('Component mounted');
  }

  componentDidUpdate(prevProps, prevState) {
    console.log('Component updated');
  }

  componentWillUnmount() {
    console.log('Component will unmount');
  }

  render() {
    return <div>My Component</div>;
  }
}
```
* Hooks (Function Components)
Hooks သည် Function Components တွင် state နှင့် lifecycle features များကို အသုံးပြုရန် React v16.8 တွင် မိတ်ဆက်ထားသည်။

* useState
useState သည် Function Components တွင် state ကို သတ်မှတ်ရန် အသုံးပြုသည်။

```
import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>Click me</button>
    </div>
  );
}
```
* useEffect
useEffect သည် component lifecycle methods များကို Function Components တွင် handle လုပ်ရန် အသုံးပြုသည်။ (e.g., data fetching, subscriptions)

```
import React, { useEffect, useState } from 'react';

function Timer() {
  const [time, setTime] = useState(new Date());

  useEffect(() => {
    const interval = setInterval(() => {
      setTime(new Date());
    }, 1000);

    return () => clearInterval(interval); // Cleanup on unmount
  }, []);

  return <div>{time.toLocaleTimeString()}</div>;
}
```
* Custom Hooks
Custom Hooks သည် reusable logic များကို Function Components တွင် အသုံးပြုနိုင်စေရန် ဖန်တီးသည်။

```
import { useState, useEffect } from 'react';

function useWindowWidth() {
  const [width, setWidth] = useState(window.innerWidth);

  useEffect(() => {
    const handleResize = () => setWidth(window.innerWidth);
    window.addEventListener('resize', handleResize);
    return () => window.removeEventListener('resize', handleResize);
  }, []);

  return width;
}

function App() {
  const width = useWindowWidth();
  return <div>Window width: {width}px</div>;
}
```
* Context API
Context API သည် application-wide data များကို component tree တစ်လျှောက်လုံး shared လုပ်ရန် အသုံးပြုသည်။

```
import React, { createContext, useContext } from 'react';

const MyContext = createContext();

function MyProvider({ children }) {
  const value = 'Hello, Context API!';
  return <MyContext.Provider value={value}>{children}</MyContext.Provider>;
}

function MyComponent() {
  const value = useContext(MyContext);
  return <div>{value}</div>;
}

function App() {
  return (
    <MyProvider>
      <MyComponent />
    </MyProvider>
  );
}
```
* Refs
Refs သည် DOM elements သို့ တိုက်ရိုက် access ရယူရန်အသုံးပြုသည်။

```
import React, { useRef } from 'react';

function TextInputWithFocusButton() {
  const inputEl = useRef(null);

  const onButtonClick = () => {
    inputEl.current.focus();
  };

  return (
    <div>
      <input ref={inputEl} type="text" />
      <button onClick={onButtonClick}>Focus the input</button>
    </div>
  );
}
```
* Error Boundaries
Error Boundaries သည် JavaScript errors များကို component tree တစ်ခုလုံး၌ catch လုပ်ပြီး, user interface ကို fail-safe state တွင် ပေါ်လာစေရန် အသုံးပြုသည်။ Class Components တွင်သာ အသုံးပြုနိုင်သည်။

```
class ErrorBoundary extends React.Component {
  constructor(props) {
    super(props);
    this.state = { hasError: false };
  }

  static getDerivedStateFromError(error) {
    return { hasError: true };
  }

  componentDidCatch(error, errorInfo) {
    console.log(error, errorInfo);
  }

  render() {
    if (this.state.hasError) {
      return <h1>Something went wrong.</h1>;
    }
    return this.props.children; 
  }
}

// Usage
function MyComponent() {
  throw new Error('I crashed!');
  return <div>My Component</div>;
}

function App() {
  return (
    <ErrorBoundary>
      <MyComponent />
    </ErrorBoundary>
  );
}
```
## 5. React တွင် Styling
React တွင် component များကို ဆွဲဆောင်မှုရှိသော design များနှင့် စတင်ဖန်တီးနိုင်ရန်အတွက် နည်းလမ်းအမျိုးမျိုးကို အသုံးပြုနိုင်သည်။

* CSS Stylesheets
CSS stylesheets ကို အသုံးပြုပြီး component များကို style ပေးနိုင်သည်။

```
import React from 'react';
import './App.css';

function App() {
  return (
    <div className="container">
      <h1>Hello, world!</h1>
    </div>
  );
}

export default App;
```
App.css ဖိုင်တွင်

```
.container {
  text-align: center;
  color: blue;
}
```
* Inline Styles
Inline styles ကို JavaScript object အနေနဲ့ ထည့်သွင်းနိုင်သည်။

```
import React from 'react';

function App() {
  const style = {
    color: 'blue',
    textAlign: 'center',
  };

  return (
    <div style={style}>
      <h1>Hello, world!</h1>
    </div>
  );
}

export default App;
```
* CSS Modules
CSS Modules သည် class name အများကြီးရှိသော large-scale applications တွင် name conflicts မဖြစ်စေရန် ကူညီပေးသည်။

```
import React from 'react';
import styles from './App.module.css';

function App() {
  return (
    <div className={styles.container}>
      <h1>Hello, world!</h1>
    </div>
  );
}

export default App;
```
App.module.css ဖိုင်တွင်

```
.container {
  text-align: center;
  color: blue;
}
```
* Styled Components
Styled Components သည် CSS-in-JS library တစ်ခုဖြစ်ပြီး JavaScript ထဲမှာ တိုက်ရိုက် CSS ကိုရေးသားနိုင်သည်။

```
npm install styled-components
```
```
import React from 'react';
import styled from 'styled-components';

const Container = styled.div`
  text-align: center;
  color: blue;
`;

function App() {
  return (
    <Container>
      <h1>Hello, world!</h1>
    </Container>
  );
}

export default App;
```
* Sass with React
Sass ကို React project တွင်အသုံးပြုနိုင်သည်။

```
npm install node-sass
```
App.scss ဖိုင်ကိုဖန်တီးပြီး

```
$primary-color: blue;

.container {
  text-align: center;
  color: $primary-color;
}
```
App.js ဖိုင်တွင်

```
import React from 'react';
import './App.scss';

function App() {
  return (
    <div className="container">
      <h1>Hello, world!</h1>
    </div>
  );
}

export default App;
```
## 6. React Router
React Router သည် React application တွင် routing နှင့် navigation ကို manage လုပ်ရန် အထောက်အကူဖြစ်သည်။

* React Router Basics
React Router ကိုစတင်အသုံးပြုရန် react-router-dom ကို install လုပ်ပါ။

```
npm install react-router-dom
```
```
import React from 'react';
import { BrowserRouter as Router, Route, Switch } from 'react-router-dom';
import Home from './Home';
import About from './About';

function App() {
  return (
    <Router>
      <Switch>
        <Route exact path="/" component={Home} />
        <Route path="/about" component={About} />
      </Switch>
    </Router>
  );
}

export default App;
```
* Route, Link, NavLink
Route, Link နှင့် NavLink များကို အသုံးပြု၍ navigation လုပ်နိုင်သည်။

```
import React from 'react';
import { BrowserRouter as Router, Route, Switch, Link, NavLink } from 'react-router-dom';
import Home from './Home';
import About from './About';

function App() {
  return (
    <Router>
      <nav>
        <ul>
          <li>
            <Link to="/">Home</Link>
          </li>
          <li>
            <NavLink to="/about" activeClassName="active">About</NavLink>
          </li>
        </ul>
      </nav>
      <Switch>
        <Route exact path="/" component={Home} />
        <Route path="/about" component={About} />
      </Switch>
    </Router>
  );
}

export default App;
```
* Dynamic Routing
Dynamic routing ကို URL parameter များဖြင့် route လုပ်နိုင်သည်။

```
import React from 'react';
import { BrowserRouter as Router, Route, Switch, useParams } from 'react-router-dom';

function User() {
  let { id } = useParams();
  return <h2>User ID: {id}</h2>;
}

function App() {
  return (
    <Router>
      <Switch>
        <Route path="/user/:id" component={User} />
      </Switch>
    </Router>
  );
}

export default App;
```
* Nested Routes
Nested routes သည် parent route အောက်တွင် child routes များရှိစေသည်။

```
import React from 'react';
import { BrowserRouter as Router, Route, Switch, Link, useRouteMatch } from 'react-router-dom';

function Topics() {
  let { path, url } = useRouteMatch();

  return (
    <div>
      <h2>Topics</h2>
      <ul>
        <li>
          <Link to={`${url}/components`}>Components</Link>
        </li>
        <li>
          <Link to={`${url}/props-v-state`}>Props v. State</Link>
        </li>
      </ul>

      <Switch>
        <Route exact path={path}>
          <h3>Please select a topic.</h3>
        </Route>
        <Route path={`${path}/:topicId`}>
          <Topic />
        </Route>
      </Switch>
    </div>
  );
}

function Topic() {
  let { topicId } = useParams();
  return <h3>Requested topic ID: {topicId}</h3>;
}

function App() {
  return (
    <Router>
      <div>
        <ul>
          <li>
            <Link to="/">Home</Link>
          </li>
          <li>
            <Link to="/topics">Topics</Link>
          </li>
        </ul>

        <Switch>
          <Route exact path="/">
            <h2>Home</h2>
          </Route>
          <Route path="/topics" component={Topics} />
        </Switch>
      </div>
    </Router>
  );
}

export default App;
```
* Redirects and Navigation
React Router တွင် redirects နှင့် navigation ကို handle လုပ်နိုင်သည်။

```
import React from 'react';
import { BrowserRouter as Router, Route, Switch, Redirect } from 'react-router-dom';

function App() {
  return (
    <Router>
      <Switch>
        <Route exact path="/">
          <h2>Home</h2>
        </Route>
        <Route path="/old-path">
          <Redirect to="/new-path" />
        </Route>
        <Route path="/new-path">
          <h2>New Path</h2>
        </Route>
      </Switch>
    </Router>
  );
}

export default App;
```
## 7. State Management
* Lifting State Up
State ကို parent component မှာ ထိန်းချုပ်ခြင်းဖြင့် child components တွင် state အခြေအနေကို ပြန်လည် share လုပ်နိုင်သည်။

```
import React, { useState } from 'react';

function App() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <Counter count={count} setCount={setCount} />
      <p>Count: {count}</p>
    </div>
  );
}

function Counter({ count, setCount }) {
  return (
    <button onClick={() => setCount(count + 1)}>Increment</button>
  );
}

export default App;
```
* Context API
Context API သည် React component များကြား data များကို props မတက်ဘဲ share လုပ်နိုင်စေသည်။

```
import React, { createContext, useContext, useState } from 'react';

const CountContext = createContext();

function App() {
  const [count, setCount] = useState(0);

  return (
    <CountContext.Provider value={{ count, setCount }}>
      <Counter />
      <Display />
    </CountContext.Provider>
  );
}

function Counter() {
  const { count, setCount } = useContext(CountContext);
  return (
    <button onClick={() => setCount(count + 1)}>Increment</button>
  );
}

function Display() {
  const { count } = useContext(CountContext);
  return <p>Count: {count}</p>;
}

export default App;
```
* Redux
Redux သည် state management library ဖြစ်ပြီး single source of truth အနေဖြင့် state ကို manage လုပ်ရန်အသုံးပြုသည်။

```
npm install redux react-redux
```
  * Actions, Reducers, Store
Actions, reducers, နှင့် store ကို အသုံးပြု၍ Redux setup လုပ်သည်။

```
import React from 'react';
import { createStore } from 'redux';
import { Provider, useDispatch, useSelector } from '
```
