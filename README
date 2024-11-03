## AXIOS

 ### Load Data Using Axios

```js
const [bookings, setBookings] = useState([]);

const url = "url";
    useEffect(() => {
        axios.get(url, {withCredentials: true})
        .then(res => {
            setBookings(res.data);
        })
    }, [url]);

```
### Post Data Using Axios

  ```js
  const user = { email };
  axios.post('url', user, { withCredentials: true })
                    .then(res => {
                        console.log(res.data)
                        if (res.data.success) {
                           console.log("Data Posted")
                        }
                    })

   ```


## Update The Data using axios

```js

   const handlesubmit = e => {
        e.preventDefault()
        const data = { name, gmail }
        // send to data server
        const url="http://localhost"
        axios.put(url,data)
        .then(data => {
           console.log(data.data)
        })  
                   
    }                 

```


### Delete

```js

const [services,setServices]=useState([])

const handleDelete = _id => {
    
        Swal.fire({
            title: 'Are you sure?',
            text: "You won't be able to revert this!",
            icon: 'warning',
            showCancelButton: true,
            confirmButtonColor: '#3085d6',
            cancelButtonColor: '#d33',
            confirmButtonText: 'Yes, delete it!'
        })
        .then((result) => {
            if (result.isConfirmed){
               axios.delete(`http://localhost:5050/user/${userr._id}`)
.then(res=>res.json())
.then(data=>{
    if(data.deletedCount>0){
        Swal.fire(
            'Deleted!',
            'Your Service has been deleted.',
            'success'
        )
        const remaining =services.filter(ser=> ser._id !== _id)
        setServices(remaining)
    }
})

            }
        
        })
}

```
