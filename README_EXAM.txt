J'ai pris les variantes Shader/Post Process et UI

Pour les mouvements du perso j'ai retiré les options de profondeur du controlleur de base du thirdperson, ainsi que celles de la camera.

Pour les pièges j'ai fait un actor avec une collision box qui trigger une fonction deal damage qui trigger dans le character une fonction On Any Damage qui update les PVs.

Pour le trou qui tue, j'ai créé une killzone qui lance une commande qui reload le level dans son OnBeginOverlap.

Pour les collectibles, c'est des actors qui appellent le character pour incrémenter le score et qui s'autodétruisent après.

Pour le post process, je l'ai mis dans le viewport du character, et je l'appelle soit quand le score s'incrémente soit quand ils prends des dégats.

Pour l'UI j'ai créé un Widget qui contient la barre de PV et le nombre du score, et je les ai bind au variables de score et de pv du character.



J'ai eu un Crash d'unreal vers 18h10, pour lequel t'es venu m'aider (encore meri btw) et qui m'as fait perdre les shaders que j'avais fait pour faire du post process custom que j'ai pas eu le temps de refaire.