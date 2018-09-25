# Julia-median
The code can get the median of **one dimension Array** <br/>
mean(x::Array)=sum(x)/length(x) <br/>
function median(x::Array)   <br/>
    if length(x)%2==0  <br/>
        X=sort!(x) <br/>
        i=length(x) <br/>
        a=Int(i/2) <br/>
        b=Int((i+2)/2) <br/>
        (X[Int(a)]+X[Int(b)])/2 <br/>
    else <br/>
        X=sort!(x)  <br/>
        i=length(x) <br/>
        X[Int((i+1)/2)] <br/>
    end  <br/>
end  <br/>
