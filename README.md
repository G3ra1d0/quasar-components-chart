![download](https://user-images.githubusercontent.com/46326067/76327323-a20d8e00-62c8-11ea-89a1-d24b53621ee6.png)
![chartjs-tutsplus](https://user-images.githubusercontent.com/46326067/76327368-ac2f8c80-62c8-11ea-8e2e-4d1e8de35332.jpg)

# quasar-components-chart

## Install
- **npm** install: `npm i quasar-components-chart --save`


### How to use
You need to import the component

```javascript
import QChart from 'quasar-components-chart'
```
Now you need to register the component
```js
import QChart from "chart.js";

export default {
  components: { QChart },
  data() {
    return {};
  }
}
```
You can use the component
```vue
<q-chart 
  identifier="myChart"
  stilo="height:30vh; width: 100%"
  :type="line"
  :labels="labels"
  :datasets="datasets"
  :options="options"
/>        
```
- identifier = ID
- stilo = CSS
- type = [Chart type](https://www.chartjs.org/)
- labels = [Labels of chart js](https://www.chartjs.org/)
- datasets = [Datasets of Chart js](https://www.chartjs.org/)
- options = [Options of Chart js](https://www.chartjs.org/)


