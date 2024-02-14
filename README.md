# Counter-app 
import React, { useState } from 'react'


const UseState2 = () => {
  const [count, setCount] = useState(0);
  const handleIncrement = () =>(
    setCount(count + 1)
  )

  const handleDecrement = () =>(
    setCount(count - 1)
  )
  const handleReset = () =>(
    setCount(0)
  )

  return (
    <div className='d-flex justify-content-start align-items-center'  style={{height:"100vh",textAlign:"center"}}> 
       <div>
        <div style={{justifyContent:"center"}}>
        <h1>COUNTERAPP</h1>
          <h1 className="text-center fs-5">{count}</h1> 
          <div className='d-flex'> 
               <button onClick={handleIncrement} className='btn btn-danger me-3'  style={{color:"white", background:"green", fontFamily:"Verdana", fontSize:"20px", marginRight:"10px"}}>Increment</button> 
              
               <button  onClick={handleDecrement} className='btn btn-danger ms-3' style={{color:"white", background:"red", fontFamily:"Verdana", fontSize:"20px", marginRight:"10px"}}>Decrement</button>
               <button  onClick={handleReset} className='btn btn-danger ma-3' style={{color:"white", background:"grey ", fontFamily:"Verdana", fontSize:"20px", marginRight:"10px"}}>Reset</button>
            </div>
        </div>
        </div> 
    </div>

  )
}

export default UseState2
