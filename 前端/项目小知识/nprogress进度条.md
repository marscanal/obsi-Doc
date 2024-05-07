
```js
//npm下载并引入
import nProgress from 'nprogress'
//修改进度条颜色
import '@/../node_modules/nprogress/nprogress.css'
//创建axios实例
const request = axios.create({
    baseURL:'/api',
    timeout:5000
})

//请求拦截器
request.interceptors.request.use((config)=>{
//每次发出请求，则进度条开始
    nProgress.start()
    return config
})

// 响应拦截器
request.interceptors.response.use((res)=>{
//接收响应，则进度条结束
    nProgress.done()
    return res.data
},(err)=>{
    return Promise.reject(new Error('faile'))
})
export default request;

```
