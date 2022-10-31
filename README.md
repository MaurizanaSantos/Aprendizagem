# Aprendizagem
Classe Disciplina.cs
using System;
namespace Edka.Sa05
{
public class Disciplina
{
public string nome { get; set; }
public DataTime DataInicial { get; set; }
public DateTime DataFinaç { get; set; }
public override string ToString()=>"&gt; $&quot;{}- - - - - - - - {} -{}&quot;;
}
 public static LIST<Dicipina> disciplinas _new List<Disciplina>
{new Disciplina{Nome="Neurociencia e, Aprendizagem",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)};
{new Disciplina{Nome="Socio emocionais",DataInicial= new DataTime(2022,08,10),DataFinal=new DataTime(2022,08,24)};
{new Disciplina{Nome="Felicidade,DataInicial= new DataTime(2022,08,32),DataFinal=new DataTime(2022,09,14)};
{new Disciplina{Nome="Teoria do Desenvolvimento Humano e da Aprendizagem",DataInicial= new DataTime(2022,09,19),DataFinal=new DataTime(2022,10,24)};
{new Disciplina{Nome="Planejamento Pedagogico",DataInicial= new DataTime(2022,08,27),DataFinal=new DataTime(2022,10,23)};
{new Disciplina{Nome="Educação Inclusiva e Cidadania",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)};
{new Disciplina{Nome="Gestão da Sala de Aula",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)};
{new Disciplina{Nome="Met.Dinãmicas e inovativas",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)};
{new Disciplina{Nome="Projeto Integrador",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)};
{new Disciplina{Nome="Avaliação Por Competência",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)};
{new Disciplina{Nome="Aprendizagem Por Competência",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)};
{new Disciplina{Nome="Prática Docente à Distânçia",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)};
{new Disciplina{Nome="Legislação e diretrizes da Educação Profissional e Tecnologica",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)};
{new Disciplina{Nome="Ambientes de Aprendizagem Inovativos",DataInicial= new DataTime(2022,08,08),DataFinal=new DataTime(2022,09,12)},
}
Classe Program.cs
using System;
using System.Collections.Generic;
using System.Linq;
namespace Edka.Sa05
{
internal class Program
{
//Dados Mock (dados para teste)
//Lista Genérica &lt; &gt;
public static List&lt;Despesa&gt; disciplinas = new List&lt;Disciplina&gt;
{
new Disciplina{Descricao=&quot;Internet&quot;,Valor=89,Vencimento=new DateTime(2022,11,15)},
new Disciplina{Descricao=&quot;Luz&quot;,Valor=99,Vencimento=new DateTime(2022,11,07)},
new Disciplinaa{Descricao=&quot;Água&quot;,Valor=150,Vencimento=new DateTime(2022,11,02) },
new Disciplina{Descricao=&quot;Gasolina&quot;,Valor=299,Vencimento=new DateTime(2022,11,11) },
new Disciplina{Descricao=&quot;Roupas&quot;,Valor=300,Vencimento=new DateTime(2022,11,20) }
};

static void Main(string[] args)
{
//Filtro LINQ
//from
//in
//select

var despesasAbaixodeCem = from d in despesas //onde?
where d.Valor &lt; 300 //condição
//orderby d.Vencimento //crescente
orderby d.Vencimento descending
select d;//selecione
foreach (var item in despesasAbaixodeCem)
{
Console.WriteLine(item);
}
Console.ReadKey();
