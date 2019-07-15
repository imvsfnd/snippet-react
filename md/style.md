#### REACT INLINE STYLE

<code>

    const style = {
      backgroundColor: "#666"
    }; 
      class App extends React.Component {
        render() {
          return (
            <div>
              <p style={style}>Lorem</p>
            </div>
          );
        }
      }
    ReactDOM.render(<App />, document.getElementById("app"));
</code>

##### style = {} 目前狀態是object

##### Reference  https://andy6804tw.github.io/2018/02/02/styling-react-components/

