# Quetion4_Dhiraj
Quetion4
<?php
function divisorSum($n) 
{

    $sum = 0;
 

    for ($i = 1; $i <= $n; ++$i) 

    {
 

        // Find all divisors of i

        // and add them 

        for ($j = 1; $j * $j <= $i; ++$j) 

        {

            if ($i % $j == 0) 

            {

                if ($i / $j == $j)

                    $sum += $j;

                else

                    $sum += $j + $i / $j;

            }

        }

    }

    return $sum;
}
 

$n = 42;

echo "\n", divisorSum($n), "\n";

$n = 147;

echo divisorSum($n), "\n";
 
?>
