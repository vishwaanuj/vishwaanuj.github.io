<script>

</script>


<div class="header">
<div class="item">{"<Home/>"}</div>
<div class="item">{"<Projects/>"}</div>
<div class="item">{"<About/>"} </div>
<div class="item">{"<Contact/>"} </div>
</div>

<style>
.header{

    display: flex;
    justify-content: space-between;
    font-size: 2.1vh;
    font-weight: 600;

    padding: 10px;
    margin:10px;
}

.item{
    transition:.2s linear;
font-style: italic;
background-color: rgb(76, 76, 76);
color:white;
padding:10px;
border-radius: 10px;
margin: 2px;

}

 .item:active{
transform: translateY(12px);
}

</style>