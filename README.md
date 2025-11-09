# do-while
^^^
string kasutajaNimi = "";
do
{
    Console.WriteLine("Palun sisesta oma kasutajanimi");
    kasutajaNimi = Console.ReadLine();
} 
while (kasutajaNimi != "user1");

if (kasutajaNimi == "user1")
{
    int ruuduSuurus = 0;

    do
    {
        Console.WriteLine("Kui suurt ruutu tahad?");
        ruuduSuurus = int.Parse(Console.ReadLine());
    } 
    while (ruuduSuurus < 0 && ruuduSuurus > 20);

    char reaKujund = '!';
    string yksRida = "";
    int tsukliMuutuja = ruuduSuurus;
    do
    {
        yksRida += "_" + reaKujund;
        tsukliMuutuja -= 1;
    } while (tsukliMuutuja != 0);
    tsukliMuutuja = ruuduSuurus;
    do
    {
        Console.WriteLine(üksRida);
        tsukliMuutuja -= 1;
    } 
    while (tsukliMuutuja != 0);

    Console.WriteLine($"Palun, siin on sinu ruut, suurusega {ruuduSuurus}x{ruuduSuurus}");
}
