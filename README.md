# Reactsyntax state
to access the value of state by calling this.props


# LifeCycle 2016

2020 version see https://zh-hant.reactjs.org/docs/react-component.html

    | getInitialState()

    | componentWillReceiveProps(props){

          setState({object})

       }

       | shouldComponentUpdate()

       | componentWillMount()

       | componentWillUpdate()

       | render()

       | componentDidMount()

       | componentDidUpdate()

        * deprecated

       | getDefaultProps

 # value accessor
 
 | this.props.__
 
 | this.state.__
 
 # JQuery
 
 https://juejin.im/post/5ac493bc51882577b45f3cfb
 
 # ES5
 
 var ReactTestUtils = require('react-dom/test-utils'); // ES5 with npm
 
 React.creatClass()
 
 
 # ES6
 
    class Counter extends React.Component {
      constructor(props) {
        super(props);
        this.state = {};
        this.method = this.method.bind(this);
      }
      componentDidMount() {
          ${this.state.count}

      }
      componentDidUpdate() {
           ${this.state.count}
      }
      method() {
        this.setState(state => ({
          count: state.count + 1,
        }));
      }
      render() {
        return (
          <div>
            <p> {this.state.count} </p>
            <button onClick={method}>
              Click me
            </button>
          </div>
        );
      }
    }







