# base-scene-image

这是一个例子组件


## Usage

### install
```javascript
 npm install wepy-swipe-delete --save
```



### props

```javascript
    props = {
      imgUrl: {
        type: String,
        default: null
      },
      index: {
        type: Number,
        default: ''
      }
    }
```	

* imgUrl 图片的url
* index 索引

### $emit

>如有$emit 在此写清楚

例如:

$emit('timeupdate', { state: 'tmeupdate' })

state: xxx状态
