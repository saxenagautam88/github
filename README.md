---------------Question 1---------------------
<?php
 $array = array(1,2,3,4,5,6,7,8,9,10);
 $count = count($array);
  $sum = 0; 
  for($i=0;$i<$count;$i++)
{ $sum += $array[$i]; }
 echo $sum ; 
 ?>
 
-----------------Question 2---------------------
<?php 
function printRepeating($arr, $size) 
{ 
	$i; 
	$j; 
	echo " Repeating elements are "; 

	for($i = 0; $i < $size; $i++) 
		for($j = $i + 1; $j < $size; $j++) 
			if($arr[$i] == $arr[$j]) 
				echo $arr[$i], " "; 
}  
$arr = array(0,1,2,3,4,5,6,7,7,8,9,10,12,12,15,16,16); 
$arr_size = sizeof($arr, 0); 
printRepeating($arr, $arr_size);  
?> 

------------------Question 3----------------------
<?php 
$arr=array(1,0,1,0);
echo (findMaxOnes(arr));    
function findMaxOnes($arr)
{
  $count=0;    
  $maxCount=0;
  for($i = 0; $i < $arr.length; $i++) {
  if($arr[i]==1)
  {
   count=count+1;   
  }
    else{count=0;}
   }
maxCount=count > maxCount ? count : maxCount;  
}
return maxCount;
}
?>
---------------------Question 4---------------------
<?php
function printPairs($arr, $n, $sum)
{
	$count = 0; 
	for ($i = 0; $i < $n; $i++)
		for ( $j = $i + 1; $j < $n; $j++)
			if ($arr[$i] + $arr[$j] == $sum)
				echo "(", $arr[$i], ", ",
						$arr[$j], ")", "\n";
}
$arr = array (1, 5, 7, -1, 5);
$n = sizeof($arr);
$sum = 6;
printPairs($arr, $n, $sum);
?>
---------------------Question 5---------------------
create table users(username varchar(50), password varchar(50));
--------------------------------
create table address(user_id number(10),
STREET number(10),
PINCODE	NUMBER(10),
COUNTRY	VARCHAR2(4000),
STATE	VARCHAR2(4000),
PHONE_NUMBER number(10) ,
foreign key(user_id) REFERENCES user_table(user_id)
);





