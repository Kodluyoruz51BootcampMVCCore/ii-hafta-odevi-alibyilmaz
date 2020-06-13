# II Hafta (6-7 Haziran) Ödevleri 

#### Github'ın Gitflow'u ile diğer yaklaşımları arasındaki fark nedir? ( gitflow vs ..) 
#### repo içinde github vs. gitflow https://github.com/Kodluyoruz51BootcampMVCCore/ii-hafta-odevi-alibyilmaz/blob/master/gthubflow-vs-gitflow.md

#### izlendi -[Git and GitHub with Briana Swift](https://www.youtube.com/playlist?list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4) Youtube Listesi incelensin. (11 Video) 

####  Merge pull request, Create a merge commit, Squash and merge,Rebase and merge altında ne fark var?
#### Merge commits
Will keep all commits history of the feature branch and move them into the master branch
Will add extra dummy commit.
#### Rebase and merge
Will append all commits history of the feature branch in the front of the master branch
Will NOT add extra dummy commit.
#### Squash and merge
Will group all feature branch commits into one commit then append it in the front of the master branch
Will add extra dummy commit.
src: https://stackoverflow.com/a/58608571

 
####  issue ve #pull request de id ler neden artıyor farklı sekmeler olmasına rağmen?

#### Answer: Note: If an issue is opened via a GitHub App, the response will include the performed_via_github_app object with information about the GitHub App. src: https://developer.github.com/v3/issues/

#### başlandı [Ramp up on Git and GitHub](https://lab.github.com/githubtraining/paths/ramp-up-on-git-and-github) 

#### Aspnetboilerplate ve yan ürünler araştırması. [AspNet Boilerplate - Web Application Framework](https://aspnetboilerplate.com/)

#### Şirketin tüm yan ürünleri ve open source repoları : https://volosoft.com/open-source 

#### başlandı hackerRank.com --> [30 Days Of Code](https://www.hackerrank.com/domains/tutorials/30-days-of-code) 

#### Razor Pages Nedir?
ASP.NET Core Razor Pages is a page-focused framework for building dynamic, data-driven web sites with clean separation of concerns. Based on the latest version of ASP.NET from Microsoft - ASP.NET Core, Razor Pages supports cross platform development and can be deployed to Windows, Unix and Mac operating systems.

The Razor Pages framework is lightweight and very flexible. It provides the developer with full control over rendered HTML. The framework is built on top of ASP.NET Core MVC, and is enabled by default when MVC is enabled in a .NET Core application. Razor Pages is the recommended framework for cross-platform server-side HTML generation on .NET Core. You do not need to have any knowledge or understanding of MVC to work with Razor Pages.
src: https://www.learnrazorpages.com/#:~:text=link,Unix%20and%20Mac%20operating%20systems.

### -  4 Farklı Projede Yapılacak *Change Authentication* :
#### repo içinde  -  No Authentication https://github.com/Kodluyoruz51BootcampMVCCore/ii-hafta-odevi-alibyilmaz/tree/master/NoAuthentication
 
#### repo içinde -  Individual User Account https://github.com/Kodluyoruz51BootcampMVCCore/ii-hafta-odevi-alibyilmaz/tree/master/Login1
 
#### repo içinde -  Work or School Accounts https://github.com/Kodluyoruz51BootcampMVCCore/ii-hafta-odevi-alibyilmaz/tree/master/Login2
 
#### repo içinde  -  Windows Authentication https://github.com/Kodluyoruz51BootcampMVCCore/ii-hafta-odevi-alibyilmaz/tree/master/Login3

#### Ayarlardaki Output kısmındaki Console Application nedir? diğerleri arasında fark nedir? [Ders Akışındaki 6. Madde'yi inceleyin.] ( araştırma ödev verildi ).

#### Console applications 
Console apps are light weight programs run inside the command prompt (DOS) window. They are commonly used for test applications.
Console-based applications include Alpine (an e-mail client), cmus (an audio player), Irssi (an IRC client), Lynx (a web browser), Midnight Commander (a file manager), Music on Console (an audio player), Mutt (an e-mail client), nano (a text editor), ne (a text editor), newsbeuter (an RSS reader), and ranger (a file manager).

#### Windows Application 
Windows Applications are form based standard Windows desktop applications for common day to day tasks. Microsoft word is an example of a Windows application.
src: https://stackoverflow.com/a/58160465

#### c# json serialize / deserialize
serialize ya da serialization, bir datayı kolayca ulaşılabilir hala getirmek ya da bir datayı platform bağımsız hale getirmektir(json,xml,binary).
Bu durumda deserialize ise: Ulaşılabilir hale gelmiş datayı tekrardan hangi dilde yazıyorsak o dildeki objeye çevirmektir. 
src: https://medium.com/@emrebalcii94/messagepack-nedir-serialize-deserialize-y%C3%B6ntemleri-neden-%C3%B6nemlidir-836a5f85b7b8
Microsoft'un kod örneklerinin de bulunduğu konuyla alakalı bir dökümanı: https://docs.microsoft.com/tr-tr/dotnet/standard/serialization/system-text-json-how-to 

#### MVC vs MVVM, MVP vs MVW vs MVU Pattern arasındaki farkı araştır

#### MVC
MVC'nin en büyük avantajı sorumlulukları Model,View ve Controller’a temiz bir şekilde dağıtmasıdır. Controller’lar uygulamanın akışını kontrol ederler, nerede neyin nasıl yapılmasına gerektiğine karar verirler. View sadece kendisinin nasıl update olacağına ilişkin business’ı içerir, Model’i oluşturur ve kullanıcıya gösterir. View uygulamayla ilgili hiç bir logic içermediğinden dolayı farklı platformlar (Windows, Web) için aynı controller’ı kullanan birden fazla View olabilir (Daha öncede dediğim gibi her zaman okadar kolay olmayabiliyor).
Ama dezavantajlarıda yok değil. View ile Model arasındaki observer ilişkisi ilk bakışta karışık gelebilir, View’in güncellenmesi için, Controller’ın Model’i güncellemesi gerek ki Model’de değiştiğini View’e bildirebilsin. Ayrıca .Net gibi modern programlama ortamları User Inputlar’ın eventlerini zaten kendileri handle ediyorlar, mesela buton’a tıklandığıda veya textbox’ın text’i değiştiğindeki eventler gibi.yapabiliyor vs. 
#### MVP (Model-View-Presenter)
MVP Pattern’i aslında MVC’den evrilmiş bir pattern, sadece bağımlılıklar değişiyor ve Controller’ın yerine Prenseter (ki bu durumda kendisine hala Controller denebiliyor) geliyor.
MVVM Pattern’i hakkında bilgi vermeden önce Presentation Model hakkında bilgi vermek istiyorum. Çünkü MVVM dediğimiz şeye; WPF ve Silverlight için Prensentation Model diyebiliriz.
src: https://denizirgin.com/mvc-mvp-ve-mvvm-patternleri-aa7d1011daff

#### MVVM PATTERN
Model - View - ViewModel is introduced by Microsoft in order to simplify the event-based implementation in the user interface. MVVM is used to extract the state and behaviour of view which allows us to separate the UI form business logic. In the MVVM the input begins with the view, not the viewModel. MVVM supports two- way data binding between view and the ViewModel. In MVVM the view holds the reference to the view Model. The ViewModel has no data about the view. In MVVM the view has no idea about the model because the view knows its model is the ViewModel.

src: https://www.eidk.org/diffrence-between-mvp-mvc-mvvm.html

#### Using a Model-View-Update (MVU)
-like approach with WebSharper UI. As you will see, WebSharper UI can implement a number of different styles of reactive UI programming easily.
Model - the state.
View - the presentation (HTML) of the state.
Update - describes how to update the state.
src: https://dzone.com/articles/part-2-model-view-update-mvu-style-apps-with-websh
