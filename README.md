## Chef Solo + Vagrant demo for DevOps course

Устанавливаем gems из Gemfile с помощью bundler
```bash
$ bundle
```

Инициализируем стандартные chef директории для создания наших рецептов
```bash
$ knife solo init .
```

Устанавиливаем нужные cookbooks из Cheffile (в нашем случае - стандартный nginx)
```bash
$ librarian-chef install
```

Перемещаем уже готовую ноду в директорию nodes
```bash
$ mv vagrant.json nodes/vagrant.json
```

Создаем Vagrant image
```bash
$ vagrant up
```