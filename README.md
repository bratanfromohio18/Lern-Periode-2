# Grob Planung
✍️ Leandro Küng

✍️ Bis zum 19.12.2023

# Leit-Satz
✍️ Ich möchte in dieser Lernperiode, das programmieren üben. Jedoch will ich zuerst die Module gut abschliessen und in den Stunden vor der Abgabe nochmal an den Modulen arbeiten, bevor ich mit einem Projekt beginne. Das Programmierprojekt, soll etwas sein, das man gebrauchen kann und ein Projekt, in dem ich viel lerne. Ich möchte sicher nochmal die Arrays anschauen. Ich möchte in dieser Lernperiode mich noch mehr anstrengen als in der letzten damit ich viel dazu lerne. Ich möchte jedoch zuerst das Modul 319 gut abschliessen und das Modul 431 ebenfalls gut abschliessen. Das Projekt das ich machen will soll aus rechnen bestehen. Es soll gut gebrauchlich sein.
(107 Wörter)

# Arbeitspakete für den 24.10.2023

- [ x ] Heute möchte ich den Auftrag 1731 im Modul 431 fertig machen.
- [ X ] Heute möchte ich den ExZ 1732 Auftrag machen.
- [ ] Heute möchte ich das Modul 431 abschliessen

Heute habe ich an dem Modul weitergearbeitet und ich habe die Aufträge fertig gemacht. Heute habe ich produktiv gearbeitet und ich war sehr konzentriert. Ich habe das Modul fast abgeschlossen und ich muss nicht mehr viel machen. Ich habe das Gefühl, das die Pausen notwendig sind weil ich sonst nicht so gut arbeiten kann. Ich brauche sie um mich kurz wieder aufzufrischen und das hat heute sehr gut funktioniert. (71 Wörter)

# Arbeitspakete für den 31.10.2023

- [ ] Ich möchte ein Plattformspiel programmieren.
- [X] Ich möchte Operatoren repetieren.
- [X] Ich möchte mich mit dem Projekt auseinandersetzen, dass uns die Kantilehrer gegeben haben.
- [X] Ich möchte Arrays repetieren.

Heute habe ich angefangen eine Website zu programmieren. Ebenfalls habe ich heute die Operatoren repetiert. Ich habe mich mit meinem Notenrechner auseinandergesetzt und ein bisschen überarbteitet. Ich habe ebenfalls die Arrays repetiert und mir die Theorie von den Arrays angeschaut, studiert und versucht umzusetzen. Ich habe heute gut gearbeitet habe ich das Gefühl und ich möchte so weiter arbeiten. (59 Wörter)

# Arbeitspakete für den 07.11.2023

- [X] Ich möchte die Arrays in mein Programm einbringen.
- [X] Ich möchte ein Notizen Programm programmieren.
- [ ] Ich möchte das Notenrechnerprogramm erweitern.

Ich habe heute an meinem Notizenprogramm gut gearbeitet und ich konnte es weiterentwickeln. Ich finde heute habe ich allgemein sehr konzentriert gearbeitet und ich konnte auch mehr schlafen weil wir Homeschooling hatten. Wenn wir nämlich kein Homeschooling haben ist es für mich immer stressig weil ich immer eine halbe Stunde zu früh in der BBB bin. Das macht für mich einen sehr grossen Unterschied weil ich mich zu Hause besser konzentrieren kann.

# Arbeitspakete für den 14.11.2023
- [X] Ich möchte mit einem Buchungsatztrainer anfangen.
- [X] Ich möchte das Projekt das wir angefangen haben ein bisschen erweitern
- [ ] Ich möchte das Notizen programm erweitern

  Heute haben ich und meine Gruppe an dem Programmierprojekt gearbeitet. Wir sind sehr gut voran gekommen und wir konnten gute Sachen programmieren. Der           Buchungssatztrainier ist gut aufgebaut und er hat eine gute Struktur. Er wurde gut bearbeitet und wir sind heute weit gekommen.

# Arbeitspakete für den 21.11.23

- [X] Ich möchte am Programmierprojetk weiterarbeiten
- [X] Ich möchte die Datentypen repetieren
- [ ] Ich möchte den Notenrechner erweitern

Heute habe ich und meine Gruppe an dem Programmierprojekt weitergerarbeitet. Wir müssen für das Programmierprojekt einen Server erstellen und wir haben viel recherchiert. Es ist sehr komplex und sehr schwierig. Ich finde weil wir zu Hause gearbeitet haben, sind wir mehr voran gekommen und wir konnten besser arbeiten als sonst. Hier unten sehen sie noch den Code zum Server an dem wir gerade arbeiten.

using System;
using System.Text;
using SimpleTCP;




namespace Test
{
    class Program
    {
        static void Main(string[] args)
        {
            var server = new SimpleTcpServer();
            
            server.ClientConnected += (sender, e) =>
            Console.WriteLine($"Client ({e.Client.RemoteEndPoint}) connected!");

            server.ClientDisconnected += (sender, e) =>
            Console.WriteLine($"Client ({e.Client.RemoteEndPoint}) disconnected!");

            server.DataReceived += (sender, e) =>
            {
                var ep = e.TcpClient.Client.RemoteEndPoint;
                var msg = Encoding.UTF8.GetString(e.Data);
                Console.WriteLine($"Received message from {ep}: \"{msg}\".");
                e.Reply(Encoding.UTF8.GetBytes("Hello back!"));
            };

            server.Start(5000);

            server.Broadcast(Encoding.UTF8.GetBytes("Message to everyone!"));

            Console.ReadLine();


        }
    }

}

# Arbeitspakete für den 28.11.2023

- [X] Heute arbeiten wir am Programmierprojekt
- [X] Heute machen wir den Code um die textdatei einzulesen
- [X] Heute arbeiten wir am Servercode

Heute haben wir an dem Programmierprojekt weitergearbeitet und wir haben den Code geschrieben für das Programmierprojekt. Heute haben wir sehr Produktiv gearbeitet und ich glaube das es am Schlaf liegt. Durch mehr schlaf sind wir produktiver.

# Arbeitspakete für den 5.12.2023



      
