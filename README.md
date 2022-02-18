# 18.02.22

    <?php
    function nav($item)
    {$items=[
        "index.php" => "Главная"
        "login.php" => "Вход"
        "registr.php" => "Регистрация"
        "admin.php" => "Администрирование"
        "lk.php" => "Личный кабинет"
        "logout.php" => "Выход"

    ];
    echo "<nav>";
    $i = 0 ;
    foreach($items as $key => $value) ; 
{ if($i == $item)
    echo "<a href='$key'class='active>$value</a>";
    else
    echo "<a href='$key'class='active>$value</a>";
    $i++;
}
echo "</nav>";
    }
?>

<?php		
		include 'nav.php';
		nav(2);
		?>
		<div class="register">
		<form action="registeraction.php" class="form" method="POST">
		<input type="text" placeholder="ФИО" name="fio">
		<input type="text" placeholder="логин" name="login">
		<input type="email" placeholder="email" name="email">
		<input type="password" placeholder="пароль" name="password">
		<input type="password" placeholder="еще раз пароль" name="confirm">
		<label><input type="checkbox">Согласие на обработку персональных данных/label>
		<button>Регистрация</button>
		</form>
		</div>
		</body>
		</html


</body>
</html>
