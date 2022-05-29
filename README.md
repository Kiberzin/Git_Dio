package PPO_pct;

public class contaPoupanca extends Conta {


}
=========================================================================================================================================================================

package PPO_pct;

public interface IConta {

    void sacar (double valor);
    void depositar (double valor);
    void transferir (double valor, Conta contaDestino);

}
=========================================================================================================================================================================


package PPO_pct;

public class contaCorrente extends Conta {

    private static final int SEQUENCIAL = 1;


    public contaCorrente() {
        super.agencia = Conta.AGENCIA_PADRAO;
        super.numero = SEQUENCIAL;
    }

}
=========================================================================================================================================================================


package PPO_pct;

public abstract class Conta implements IConta {
    protected static final int AGENCIA_PADRAO = 0001;
    private static final int SEQUENCIAL = 1;
    protected int agencia;
    protected int numero;
    protected double saldo;

    public Conta() {
        this.agencia = Conta.AGENCIA_PADRAO;
        this.numero = SEQUENCIAL;
    }

    public int getAgencia() {
        return agencia;
    }

    public int getNumero() {
        return numero;
    }

    public double getSaldo() {
        return saldo;
    }

    public void secar() {

    }

    public void depositar() {

    }

    public void transferir() {

    }

    @Override
    public void sacar(double valor) {

    }

    @Override
    public void depositar(double valor) {

    }

    @Override
    public void transferir(double valor, Conta contaDestino) {

    }
}

=========================================================================================================================================================================


package PPO_pct;

public class banco {
    private String nome;

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }
}

=========================================================================================================================================================================


package PPO_pct;

public class cliente {

    private String nome;
}
