# access-token-repo-push
Github personel access token hatası çözümü

<html>
    <head>
        <title>Github personel access token hatası çözümü</title>
    </head>
    <body>
        <h1>Github personel access token hatası çözümü</h1>
        <p> git clone https://github.com/ismailgultekin/github-new-access-token-repo-push.git <br></p>
    <p>Terminalden komutlarımızı girelim:</p>
    <ul>
        <li>git status</li>
        <li>git init</li>
        <li>git add .</li>
        <li>git commit -m "ilk Dosyaları yükledim"</li>
        <li>git branch -M main</li>
        <li>git remote add access https://repoadresiniz.git</li>
        <li>git push -u access main</li>
    </ul>
    <div class="idnote">Böyle bir hata alırsak "Support for password authentication was removed on August 13, 2021. Please use a personal access token instead."</div>
    <p>Buradaki sayfayı ziyaret etmelisiniz: https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/</p>
    
    <h2>Personel Access Token Hatasının Çözümü</h2>
    <ul>
        <li>1) Github profilinde settings bölümünü açalım</li>
        <li>2) Developers Settings tıklayalım</li>
        <li>3) Personel Access Token</li>
        <li>4) Generate New Token linkine tıklıyoruz</li>
        <li>5) Açılan formdan Gün süresini ve yetkileri belirleyoruz</li>
        <li>6) Formun altındaki Generate Token butonuna basarak oluşturuyoruz.</li>
    </ul>
    <p>Terminalden ilk olarak git remote --v kodumuz ile kontrol edelim. <br>
        Eğer bunlar mevcut ise <br>
        "origin	https://github.com/ismailgultekin/github-new-access-token-repo-push.git (fetch)
        origin	https://github.com/ismailgultekin/github-new-access-token-repo-push.git (push)"
       <br> Tekrar git push -u access main kodumuzu girelim</p>
    <div class="idnote">
        Böyle bir hata alırsak Updates were rejected because the tip of your current branch is behind
    </div>   
    <p>Terminalden yazacağımız komut: </p>
    <pre>git push -f origin main</pre>
    <p>Kodlar çakışma yaptığı için kaynaklanıyor. Şimdi yüklendiğini göreceksiniz.</p>
    <div>Web yazılım üzerine makalelerimi kişisel bloğumdan takip edebilirsiniz. <a href="https://ismailgultekin.com">İsmail Gültekin</a></div>
    </body>
</html>