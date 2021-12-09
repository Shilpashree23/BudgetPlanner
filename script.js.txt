product=new Array();
price=new Array();
function add()
{
    var c=parseInt(prompt("Enter the number of products"));
    for(let i=0;i<c;i++)
    {
    var s=prompt("Enter the product name");
    product.push(s);
    var t=parseInt(prompt("Enter the price of the product"));
    price.push(t);

    }
    for(let i=0;i<c;i++)
    {
    document.getElementById("product").innerHTML=(product+"<br>");
    document.getElementById("price").innerHTML=(price+"<br>");
    }
}

function Sum1()
{
    var sum=0;
    for(let i=0;i<price.length;i++){
    sum=sum+price[i];
    }
    document.getElementById("sum1").innerHTML="The Total Budget Of THe Month Is" +sum;
}