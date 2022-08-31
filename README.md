# Veterinaria_jhonatan_Nanez

print("BIENVENIDO AL PROGRAMA DE VETERINARIA JHONATAN FRANKY NANEZ MUNOZ")

#manejo de objetos
class Mascota:
    # atributos
    nombreMascota=''
    fechaNacimiento=''
    raza=''
    color=''
    observaciones=''

    #constructor
    def __init__(self, nombreMascota, fechaNacimiento,raza,color,observaciones,tipoMascota):
        self.nombreMascota=nombreMascota
        self.fechaNacimiento=fechaNacimiento
        self.raza=raza
        self.color=color
        self.observaciones=observaciones

        self.tipoMascota=tipoMascota # Creacion de atributo nuevo
    #metodos
    def registrarMascota(self):
        mascotaParaCrear={}
        idMascota=input('digite el Id de la mascota: ')
        if idMascota in Mascota:
            mascotaParaCrear[idMascota]=Mascota.nombreMascota
            print(mascotaParaCrear)
        else:
            print('Existe una mascota con el ID')

    def actulizarMascota(self):
        self.velocidad =self.velocidad+self.aceleracion
        return "Se actualizo la mascota exitosamente"
        
    def ConsultarMascota(registrarMascota):
        return "La consulta de la mascota es: "

class Cliente:
    # atributos
    nombres=''
    apellidos=''
    documento=''
    celular=''
    direccion=''
    correo=''

    #constructor
    def __init__(self,nombres,apellidos,documento,celular,direccion,correo,tipoDocumento):
        self.nombres=nombres
        self.apellidos=apellidos
        self.documento=documento
        self.celular=celular
        self.direccion=direccion
        self.correo=correo

        self.tipoDocumento=tipoDocumento  #Creacion de atributo nuevo

    #metodos
    def registrarCliente(self):
        clienteParaRegistro={}
        idCliente=input('digite el Id del cliente: ')
        if  idCliente in Cliente:
            clienteParaRegistro[idCliente]=Cliente.nombres
            print(clienteParaRegistro)
        else:
            print('Existe una mascota con el ID')


    def actulizarCLiente(self):
        return "Se actualizo el cliente exitosamente"

        #cosultar
    def ConsultarCLiente(self,registrarCliente):
        return "La consulta del cliente es: "

class Vacuna:
    # atributos
    nombreVacuna=''
    cantVacunas=''
    fechaVacuna=''
    fechaProxima=''
    farmaceutica=''

    #constructor
    def __init__(self,nombreVacuna,cantVacunas,fechaVacuna,fechaProxima,farmaceutica):
        self.nombreVacuna=nombreVacuna
        self.cantVacunas=cantVacunas
        self.fechaVacuna=fechaVacuna
        self.fechaProxima=fechaProxima
        self.farmaceutica=farmaceutica

    #metodos
    def registrarVacuna(self):
        registrarParaReserva={}
        idReserva=input('digite el Id de la vacuna: ')
        if idReserva in Vacuna:
            registrarParaReserva[idReserva]=Vacuna.nombreVacuna
            print(registrarParaReserva)
        else:
            print('Existe una vacuna con el ID')
             
    def eliminarVacuna(self):
        return "se elimino la vacuna exitosamente"

        #cosultar
    def ConsultarVacuna(self,registroVacuna):
        return "La consulta de la vacuna es: "

class Consulta:
    # atributos
    nombreConst=''
    fecha=''
    sintomas=''
    peso=''
    diagnostico=''

    #constructor
    def __init__(self,nombreConst,fecha,sintomas,peso,diagnostico):
        self.nombreConst=nombreConst
        self.fecha=fecha
        self.sintomas=sintomas
        self.peso=peso
        self.diagnostico=diagnostico

    #metodos
    def registrarConsulta(self):
        registrarParaReserva={}
        idReserva=input('digite el Id de la consulta: ')
        if idReserva in Consulta:
            registrarParaReserva[idReserva]=Consulta.nombreConst
            print(registrarParaReserva)
        else:
            print('Existe una consulta con el ID')
             
    def actulizarConsulta(self):
        return "Se elimino la vacuna exitosamente"

        #cosultar
    def eliminarConsulta(self,registroConsulta):
        return "La consulta de la vacuna es: "

class Reserva:
    # atributos
    fechaResv=''
    cantResv=''
    nombreResv=''
    descripcion=''
    cupoDisp=""

    #constructor
    def __init__(self,fechaResv,cantResv,nombreResv,descripcion,cupoDisp):
        self.fechaResv=fechaResv
        self.cantResv=cantResv
        self.nombreResv=nombreResv
        self.descripcion=descripcion
        self.cupoDisp=cupoDisp

    #metodos
    def registrarReserva(self):
        registrarParaReserva={}
        idReserva=input('digite el Id de la reserva: ')
        if idReserva in Reserva:
            registrarParaReserva[idReserva]=Reserva.nombreResv
            print(registrarParaReserva)
        else:
            print('Existe una reserva con el ID')
             
    def actualizarReserva(self):
        return "Se actualizo la reserva exitosamente"

        #cosultar
    def ConsultarReserva(self,registrarReserva):
        return "La consulta de la reserva es: "
