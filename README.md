# La Quiniela de Alfonsina

Invitación interactiva de baby shower: nueve apuestas sobre cómo va a nacer
Alfonsina, con puntaje por cercanía y podio automático de los tres que más se
acercaron.

La página es un único `index.html` sin dependencias ni proceso de build. Las
apuestas se guardan en una función de Supabase; acá no hay ninguna clave ni
dato personal. La zona de organizadora se abre con un token que viaja en la
URL y que no está en este código.

## El workflow de mantener despierto

Supabase duerme los proyectos gratis tras unos días sin consultas, y despertarlo
a mano requiere entrar al panel. `.github/workflows/mantener-despierto.yml` le
manda una consulta inofensiva cada dos días para que eso no pase mientras la
quiniela está abierta.

Ojo: GitHub apaga los workflows programados si el repositorio pasa 60 días sin
actividad, y las corridas automáticas no cuentan como actividad. Si llega ese
aviso por mail, alcanza con hacer cualquier cambio acá para reiniciar la cuenta.
