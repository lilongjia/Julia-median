# Julia-median
The code can get the median of **one dimension Array** <br/>
mean(x::Array)=sum(x)/length(x) <br/>
function median(x::Array)   <br/>
&ensp;&ensp;&ensp;&ensp;    if length(x)%2==0  <br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;        X=sort!(x) <br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;        i=length(x) <br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;        a=Int(i/2) <br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;        b=Int((i+2)/2) <br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;        (X[Int(a)]+X[Int(b)])/2 <br/>
&ensp;&ensp;&ensp;&ensp;    else <br/>
&ensp;&ensp;&ensp;&ensp;        X=sort!(x)  <br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;        i=length(x) <br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;       X[Int((i+1)/2)] <br/>
&ensp;&ensp;&ensp;&ensp;    end  <br/>
end  <br/>
