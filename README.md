# Todo-List app

Notre application a pour but de faciliter le travail et l'organisation de nos utilisateurs à travers des to-do-lists.

### Getting Started

* Téléchager ou cloner l'application
* Utiliser node pour installer jasmine
```
npm install
```
* Ouvrir le fichier index.html dans votre navigateur


## Running the tests

Une série de tests unitaires est mise à votre disposition. Pour les utiliser il suffit d'ouvrir le fichier SpecRunner.html se trouvant dans le dossier 'test'.

### Break down into end to end tests

Cette série de tests permet de vérifier le bon fonctionnement des différents fonctionnement de nos to-do lists. Pour cela on utilise jasmine.
```
it('should show completed entries', function () {
  var todo = {title: 'my todo', completed: true};
  setUpModel([todo]);

  subject.setView('#/completed');

  expect(view.render).toHaveBeenCalledWith('setFilter', 'completed');
  expect(view.render).toHaveBeenCalledWith('showEntries', [todo]);
});
```

## Authors

* **Oscar Godson** - *Initial work* -
* **Christoph Burgmer** - *Refactored* -
* **Emilio Cadario** - *P8* -



## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

