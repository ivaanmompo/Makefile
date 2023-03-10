actualizacion:
	@echo "Actualizamos los repositorios..."
	sudo apt update
	sudo apt upgrade
	sudo apt install git

.git:
	@echo "Haciendo el repositorio de Git..."
	git init


install:
        @echo "Instalando Eclipse..."
        wget https://eclipse.org/downloads/download.php?file=/technology/epp/do>
        tar -zxvf eclipse.tar.gz
        rm -f eclipse.tar.gz
        @echo "Instalación completada"

add: .git
        git add .

commit: add
	git commit -a -m "Primer Commit"

update:
	@echo "Comprobando si hay actualizaciones..."
	git pull
	@echo "Actualizado"

uninstall:
	@echo "Desinstalando Eclipse..."
	rm -rf eclipse
	@echo "Desinstalación completada"

clean:
	@echo "Limpiando archivos innecesarios..."
	rm -f *.o
	rm -f *.out
	rm -f *.exe
	rm -f core
	find . -type f -name '*.swp' -delete
	@echo "Limpieza completada"

delete:
	@echo "Eliminando archivos generados..."
	rm -rf *.o
	rm -rf *.out
	rm -rf *.exe
	rm -rf core
	rm -rf ./bin
	rm -rf ./build
	@echo "Eliminación completada"
