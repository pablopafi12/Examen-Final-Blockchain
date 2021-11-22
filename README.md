pragma solidity 0.8.7;

contract Bank
{
    Definimos la variable bal, la cual nos servirá para almacenar el balance
    
    int bal;
    
    Creamos un constructor
    constructor() public
    {
    //Le asignamos un valor 1 a la variable balance
        bal = 1;
    }
    //Creamos la funcion getBalance, la cual nos servirá para revisar cual es nuestro balance actual
    function getBalance() view public returns(int)
    {
    //Pedimos la variable bal
        return bal;
    }
    //Creamos la funcion retirar, la cual nos servirá para restar la catidad ingresada a nuestro balance
    function retirar(int amt) public
    {
    //Realizamos el retiro
        bal = bal - amt;
    }
    //Creamos la funcion retirar, la cual nos servirá para sumar la catidad ingresada a nuestro balance
    function depositar(int amt) public
    {
    //Realizamos el retiro 
        bal = bal + amt;
    }
}
