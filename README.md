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

- [X] Heute Arbeite ich am Finanzenrechner
- [X] Heute arbeite ich an dem Datenmodell
- [ ] Heute arbeite ich beim Modul 162 und lerne ein bisschen.

Heute habe ich einen Finanztrainer angefangen und ich bin schon weit gekommen. Ich habe mit Warenbestand und Warenertrag gearbeitet und ich habe ebenfalls mit Warenaufwand gearbeitet. Man kann entscheiden ob man den Gewinn ausrechnen will oder ob man den aktuellen Warenbestand ausrechnen will. Dazu will ich das man die Buchungssätze speichern kann und auch eine Bilanz machen kann. Ich will mich mit dem Speichern ausseinander setzen und ich will schauen wie man eine Bilanz machen könnte

# Arbeitspakete für den 12.12.2023

- [ ] Ich möchte in meinem Finanzprogramm eine Bilanz erstellen
- [X] Ich möchte das ich mein eingegebens in dem Finanazprogramm speichern kann.
- [X] Ich möchte lernen für das Modul 162
      
Ich habe an meinem Informatikprojekt weitergearbeitet und die restliche Zeit habe ich mit Modul lernen verbracht. Ich habe am Modul 162 bisschen weitergearbeitet und ein bisschen gelernt. Ich habe ebenfalls beim Projekt weitergearbeitet und ich konnte heute ebenfalls wieder gut arbeiten wei ich wiedermal mehr Schlaf hatte. Ich war produktiver als sonst. 


# Arbeitspakete für den 19.12.2023

- [X] Heute möchte ich an meinem Projekt weiterarbeiten
- [X] Heute möchte ich beim Modul 117 einen Auftrag erledigen
- [X] Heute möchte ich beim Modul 117 einen Auftrag erledigen

Heute habe ich ein bisschen am Modul 117 gearbeitet und ich es hat gut funktioniert. Gestern bin ich im Unterricht nicht so weit gekommen, darum musste ich heute ein bisschen nacharbeiten. Ich habe ebenfalls am Projekt gearbeitet und es hat auch gut funktioniert. Ich habe noch an einem Portfoliobeitrag gearbeitet, den man morgen abgebem muss. Er ist fertig geworden und ich habe nur an dem gearbeitet, weil ich den rest schon fertig hatte.

## Reflexion
Ich glaube, dass ich in dieser Zeit viel über Programmieren gelernt habe. Ich glaube, es war schwierig für mich, Begriffe und anderes zum Programmieren zu lernen. Ich glaube, ich könnte noch produktiver arbeiten, weil ich manchmal das Gefühl hatte, dass ich zu schnell nachgelassen und nicht weitergemacht habe. Ich glaube, ich könnte es besser machen, weil ich mich im Programmieren noch nicht ganz so sicher fühle. Ich benötige mehr Bewegung. In den Unterrichtsstunden möchte ich mich mehr konzentrieren. Ich denke, es geht besser, wenn ich Musik höre und meine Kopfhöhrer anziehe. 
