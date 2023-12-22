schema
const mongoose=require('mongoose)

const authSchme=mongoose.Schema({
   email:{type:String,required:true},
        password:{type:String,required:true}
           
},

{versionKey:false}
)
const modelUath=mongoose.model("user",authschme)
module.exports={
    authScheme
}


connection

.env mongodburl="url

db.js
const mongoose=require("mongoose")

consct connection=mongoose.connect(process.enev.mongourl)

module.export={
    connection
}
index.js
const connection=requirw("./db)

const app=express()

app.use(express.json())
app.use("/auth,authrouter)

app.listen(8080,async()=>{
    console.log("server is running)
    try{
        await connection
        console.log("connected to dn)

    }catch(err){
console.log("err")
    }
})

cost express=require("express")

const userRouter=express.router()

userRouter.get("/",(req,res)=>{
    res.send("home")
})

userRouter.post("/create",async(req,res)=>{

try{
    const posts=new modelpost(req.body)
    await posts.save()
    res.status(200).send("added new post")

}catch(err){
    res.status(400).send({"msg":serror.message})
}
})

userRouter.delete("/delete/:id,async(req,res)=>{
    const {id}=req.params

    try{
        const dleyepost=awiat modePost.findByIdAndDelete({_id:id})
        if(delepost){
            res.status(200).send(selet)
        }else{
            res.status(400).send (post not found)
        }

    }catch
})

userRouter.patch("/update/:id" ,sysnc(req,res)=>{

    const{id}=req.params
    try{
        const upade=awiat.modelpost.findOneByvIdAndUpdate({_id:id},req.body)
        if(upadte){
            
        }
    }
})


userRouyer.get("/",async(req,res)=>{

    try{
        cont getall=await modelpost.find()
        res.status(200).send(getall)
    }catch(err){
        res.status(400).send({"msg":err.message})
    }
})



let name1={
    firstname:"f"
    lasname:"b",
    printfullname:function(hometoen){
        console.log(tis)
    }
}

nameq.printfullname()

let name2={
    firstname:"g"
    lasname:"b",
  
}
name1.printfullname.call(name2,baramulla)


name1.printname.apply(name,[baramulla,lak,ir])
bind 
let bindcopy=printfullname.bind(name,"baramulla,ksjhir)

bind
getname()
console.log(10)
console.log(getname)
var x=10
function getname(){
    cnsole.lo
    
    function x(g ("hello)
}

fuction x(){
    var i=1
    setTimeout(()=>{
        console.log(i)
    },2000)
    console.log("hello)
}




