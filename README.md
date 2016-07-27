# NFe - Node.js

Projeto ABERTO e GRATUITO para criar a NFe para Node.js 

## Sumário

- Exemplo XML
- Requisitos
- Certificado Digital
- Computador
- Software
- Internet
- Campos obrigatórios e como preenchê-los:
- Dados do Emitente (você)
- Dados do Destinatário (seu cliente)
- Produto(s) ou Serviço(s) vendido(s)
- Nome do Produto ou Serviço
- Tipo
- Quantidade
- Valor Unitário
- Valor Total
- Peso Líquido Total
- Peso Bruto Total
- NCM
- CEST (Código Especificador de Substituição Tributária)
- Tributação:
- ICMS
- Situação Tributária
- Origem
- Natureza da operação
- Forma de pagamento
- CFOP (Códigos Fiscais de Operações e Prestações)
- Base de Cálculo do ICMS
- Valor Total do ICMS
- Base de Cálculo do ICMS ST
- Valor Total do ICMS ST
- Valor Total dos produtos e serviços
- Valor Total do Frete
- Valor Total do Seguro
- Valor Total do Desconto
- Outras Despesas acessórias
- Valor Total da NF-e
- Valor aproximado total de tributos federais, estaduais e municipais

# Exemplo XML FUNCIONANDO


```xml
<?xml version="1.0" encoding="utf-8"?>
<nfeProc versao="3.10" xmlns="http://www.portalfiscal.inf.br/nfe">
    <NFe xmlns="http://www.portalfiscal.inf.br/nfe">
        <infNFe Id="NFe33160405424008000441550010008644501143436782" versao="3.10">
            <ide>
                <cUF>33</cUF>
                <cNF>14343678</cNF>
                <natOp>VENDA C/ SUBST. TRIBUTARIA</natOp>
                <indPag>1</indPag>
                <mod>55</mod>
                <serie>1</serie>
                <nNF>864450</nNF>
                <dhEmi>2016-04-26T00:00:00-03:00</dhEmi>
                <dhSaiEnt>2016-04-26T09:04:00-03:00</dhSaiEnt>
                <tpNF>1</tpNF>
                <idDest>1</idDest>
                <cMunFG>3304557</cMunFG>
                <tpImp>1</tpImp>
                <tpEmis>1</tpEmis>
                <cDV>2</cDV>
                <tpAmb>1</tpAmb>
                <finNFe>1</finNFe>
                <indFinal>0</indFinal>
                <indPres>9</indPres>
                <procEmi>0</procEmi>
                <verProc>3.0.0</verProc>
            </ide>
            <emit>
                <CNPJ>05424008000441</CNPJ>
                <xNome>UNILIDER DISTRIBUIDORA S.A - FILIAL RIO</xNome>
                <xFant>FILIAL RJ</xFant>
                <enderEmit>
                    <xLgr>RODOVIA PRESIDENTE DUTRA</xLgr>
                    <nro>2251</nro>
                    <xCpl>GALPAO 1 ARM 101 E 102</xCpl>
                    <xBairro>PARQUE COLUMBIA</xBairro>
                    <cMun>3304557</cMun>
                    <xMun>RIO DE JANEIRO</xMun>
                    <UF>RJ</UF>
                    <CEP>21535501</CEP>
                    <cPais>1058</cPais>
                    <xPais>BRASIL</xPais>
                    <fone>2132662121</fone>
                </enderEmit>
                <IE>78362537</IE>
                <CRT>3</CRT>
            </emit>
            <dest>
                <CNPJ>18612364000198</CNPJ>
                <xNome>1925159 - WILLMARCRIS DROGARIA LTDA EPP</xNome>
                <enderDest>
                    <xLgr>ESTRADA DO PONTAL</xLgr>
                    <nro>7535</nro>
                    <xCpl>LOJA 06</xCpl>
                    <xBairro>RECREIO DOS BANDEIRANTES</xBairro>
                    <cMun>3304557</cMun>
                    <xMun>RIO DE JANEIRO</xMun>
                    <UF>RJ</UF>
                    <CEP>22790877</CEP>
                    <cPais>1058</cPais>
                    <xPais>BRASIL</xPais>
                    <fone>2135794222</fone>
                </enderDest>
                <indIEDest>1</indIEDest>
                <IE>79979260</IE>
                <email>farmabell.drogaria@gmail.com</email>
            </dest>
            <det nItem="2">
                <prod>
                    <cProd>100003905</cProd>
                    <cEAN>17506339394785</cEAN>
                    <xProd>ALWAYS BASICO SUAVE C/ABAS L8P7</xProd>
                    <NCM>96190000</NCM>
                    <CEST>2005000</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>CX</uCom>
                    <qCom>1.0000</qCom>
                    <vUnCom>29.5900000000</vUnCom>
                    <vProd>29.59</vProd>
                    <cEANTrib>7506339394788</cEANTrib>
                    <uTrib>UN</uTrib>
                    <qTrib>12.0000</qTrib>
                    <vUnTrib>2.4658333333</vUnTrib>
                    <vOutro>0.10</vOutro>
                    <indTot>1</indTot>
                    <nFCI>668170A3-58ED-49D7-8151-030AF36B750F</nFCI>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>5</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>20.78</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>4.16</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>67.44</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>25.92</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>1.02</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>29.59</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>0.49</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>29.59</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>2.25</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>CX C/ 12 UN -ST: 1,02 -GTIN: 17506339394785</infAdProd>
            </det>
            <det nItem="3">
                <prod>
                    <cProd>100002012</cProd>
                    <cEAN>17506295337529</cEAN>
                    <xProd>PAMP PREMIUM C HIPER G 60UN</xProd>
                    <NCM>96190000</NCM>
                    <CEST>2004800</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>CX</uCom>
                    <qCom>1.0000</qCom>
                    <vUnCom>64.2400000000</vUnCom>
                    <vProd>64.24</vProd>
                    <cEANTrib>17506295337529</cEANTrib>
                    <uTrib>CX</uTrib>
                    <qTrib>1.0000</qTrib>
                    <vUnTrib>64.2400000000</vUnTrib>
                    <vOutro>0.22</vOutro>
                    <indTot>1</indTot>
                    <nFCI>BFA4208D-6C88-44BF-83FF-D26689875838</nFCI>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>5</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>45.12</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>9.02</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>44.43</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>53.76</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>1.73</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>64.24</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>1.06</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>64.24</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>4.88</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>CX C/ 1 UN -ST: 1,73 -GTIN: 17506295337529</infAdProd>
            </det>
            <det nItem="5">
                <prod>
                    <cProd>100001906</cProd>
                    <cEAN>17506195185862</cEAN>
                    <xProd>PAMP PREMIUM C PTAO M 24UN</xProd>
                    <NCM>96190000</NCM>
                    <CEST>2004800</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>FA</uCom>
                    <qCom>1.0000</qCom>
                    <vUnCom>163.8100000000</vUnCom>
                    <vProd>163.81</vProd>
                    <cEANTrib>7506195172346</cEANTrib>
                    <uTrib>UN</uTrib>
                    <qTrib>6.0000</qTrib>
                    <vUnTrib>27.3016666667</vUnTrib>
                    <vOutro>0.58</vOutro>
                    <indTot>1</indTot>
                    <nFCI>9C94DDA5-6F24-4DA4-ADB9-61C3A103F483</nFCI>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>5</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>115.07</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>23.01</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>44.43</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>111.45</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>2.23</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>163.81</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>2.70</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>163.81</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>12.45</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>FA C/ 6 UN -ST: 2,23 -GTIN: 17506195185862</infAdProd>
            </det>
            <det nItem="6">
                <prod>
                    <cProd>2201838</cProd>
                    <cEAN>17501006745068</cEAN>
                    <xProd>PAMP T CONFORT PCTAO M 24UN</xProd>
                    <NCM>96190000</NCM>
                    <CEST>2004800</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>FA</uCom>
                    <qCom>1.0000</qCom>
                    <vUnCom>116.3900000000</vUnCom>
                    <vProd>116.39</vProd>
                    <cEANTrib>17501006745068</cEANTrib>
                    <uTrib>FA</uTrib>
                    <qTrib>1.0000</qTrib>
                    <vUnTrib>116.3900000000</vUnTrib>
                    <vOutro>0.41</vOutro>
                    <indTot>1</indTot>
                    <nFCI>EF7FF97B-75B5-4EAC-BEC6-273379B09C9E</nFCI>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>5</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>81.76</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>16.35</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>44.43</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>96.58</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>2.97</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>116.39</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>1.92</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>116.39</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>8.85</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>FA C/ 6 UN -ST: 2,97 -GTIN: 17501006745068</infAdProd>
            </det>
            <det nItem="4">
                <prod>
                    <cProd>24089</cProd>
                    <cEAN>7501009224099</cEAN>
                    <xProd>PRESTO REGULAR FEM PB 12X2UN</xProd>
                    <NCM>82121020</NCM>
                    <CEST>2006400</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>DP</uCom>
                    <qCom>1.0000</qCom>
                    <vUnCom>46.3100000000</vUnCom>
                    <vProd>46.31</vProd>
                    <cEANTrib>7501009224099</cEANTrib>
                    <uTrib>DP</uTrib>
                    <qTrib>1.0000</qTrib>
                    <vUnTrib>46.3100000000</vUnTrib>
                    <vOutro>0.16</vOutro>
                    <indTot>1</indTot>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>4</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>32.53</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>6.51</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>30.00</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>25.99</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>0.52</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>46.31</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>0.76</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>46.31</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>3.52</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>DP C/ 12 UN -ST: 0,52 -GTIN: 7501009224099</infAdProd>
            </det>
            <det nItem="1">
                <prod>
                    <cProd>132629</cProd>
                    <cEAN>7501009224181</cEAN>
                    <xProd>PRESTO ULTRAG CM OS 12X2UN</xProd>
                    <NCM>82121020</NCM>
                    <CEST>2006400</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>CT</uCom>
                    <qCom>1.0000</qCom>
                    <vUnCom>43.2200000000</vUnCom>
                    <vProd>43.22</vProd>
                    <cEANTrib>7501009224181</cEANTrib>
                    <uTrib>CT</uTrib>
                    <qTrib>1.0000</qTrib>
                    <vUnTrib>43.2200000000</vUnTrib>
                    <vOutro>0.19</vOutro>
                    <indTot>1</indTot>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>4</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>30.39</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>6.08</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>30.00</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>29.84</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>0.60</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>43.22</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>0.71</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>43.22</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>3.28</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>CT C/ 12 UN -ST: 0,60 -GTIN: 7501009224181</infAdProd>
            </det>
            <det nItem="7">
                <prod>
                    <cProd>100001886</cProd>
                    <cEAN>7506195153574</cEAN>
                    <xProd>PRESTO3 BODY SENSE PB 1X2UN</xProd>
                    <NCM>82121020</NCM>
                    <CEST>2006400</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>UN</uCom>
                    <qCom>3.0000</qCom>
                    <vUnCom>7.9100000000</vUnCom>
                    <vProd>23.73</vProd>
                    <cEANTrib>7506195153574</cEANTrib>
                    <uTrib>UN</uTrib>
                    <qTrib>3.0000</qTrib>
                    <vUnTrib>7.9100000000</vUnTrib>
                    <vOutro>0.08</vOutro>
                    <indTot>1</indTot>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>4</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>16.67</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>3.33</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>30.00</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>8.64</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>0.17</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>23.73</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>0.39</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>23.73</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>1.80</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>UN C/ 2 UN -ST: 0,17 -GTIN: 7506195153574</infAdProd>
            </det>
            <det nItem="8">
                <prod>
                    <cProd>100002458</cProd>
                    <cEAN>7702018294770</cEAN>
                    <xProd>PRESTO3 CORRIDA PB 1X2UN</xProd>
                    <NCM>82121020</NCM>
                    <CEST>2006400</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>UN</uCom>
                    <qCom>3.0000</qCom>
                    <vUnCom>7.9000000000</vUnCom>
                    <vProd>23.70</vProd>
                    <cEANTrib>7702018294770</cEANTrib>
                    <uTrib>UN</uTrib>
                    <qTrib>3.0000</qTrib>
                    <vUnTrib>7.9000000000</vUnTrib>
                    <vOutro>0.08</vOutro>
                    <indTot>1</indTot>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>4</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>16.65</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>3.33</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>30.00</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>10.94</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>0.22</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>23.70</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>0.39</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>23.70</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>1.80</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>UN C/ 1 UN -ST: 0,22 -GTIN: 7702018294770</infAdProd>
            </det>
            <det nItem="9">
                <prod>
                    <cProd>2202656</cProd>
                    <cEAN>7702018874729</cEAN>
                    <xProd>PRESTO3 REG PB 1X2UN</xProd>
                    <NCM>82121020</NCM>
                    <CEST>2006400</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>UN</uCom>
                    <qCom>3.0000</qCom>
                    <vUnCom>7.9100000000</vUnCom>
                    <vProd>23.73</vProd>
                    <cEANTrib>7702018874729</cEANTrib>
                    <uTrib>UN</uTrib>
                    <qTrib>3.0000</qTrib>
                    <vUnTrib>7.9100000000</vUnTrib>
                    <vOutro>0.08</vOutro>
                    <indTot>1</indTot>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>4</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>16.67</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>3.33</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>30.00</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>9.95</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>0.20</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>23.73</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>0.39</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>23.73</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>1.80</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>UN C/ 1 UN -ST: 0,20 -GTIN: 7702018874729</infAdProd>
            </det>
            <det nItem="10">
                <prod>
                    <cProd>100003838</cProd>
                    <cEAN>7506339337525</cEAN>
                    <xProd>PRESTO3 SENSI PB 1X2UN</xProd>
                    <NCM>82121020</NCM>
                    <CEST>2006400</CEST>
                    <CFOP>5403</CFOP>
                    <uCom>UN</uCom>
                    <qCom>3.0000</qCom>
                    <vUnCom>7.9100000000</vUnCom>
                    <vProd>23.73</vProd>
                    <cEANTrib>7506339337525</cEANTrib>
                    <uTrib>UN</uTrib>
                    <qTrib>3.0000</qTrib>
                    <vUnTrib>7.9100000000</vUnTrib>
                    <vOutro>0.08</vOutro>
                    <indTot>1</indTot>
                </prod>
                <imposto>
                    <vTotTrib>0.00</vTotTrib>
                    <ICMS>
                        <ICMS70>
                            <orig>4</orig>
                            <CST>70</CST>
                            <modBC>3</modBC>
                            <pRedBC>30.00</pRedBC>
                            <vBC>16.67</vBC>
                            <pICMS>20.00</pICMS>
                            <vICMS>3.33</vICMS>
                            <modBCST>4</modBCST>
                            <pMVAST>30.00</pMVAST>
                            <pRedBCST>25.00</pRedBCST>
                            <vBCST>8.93</vBCST>
                            <pICMSST>20.00</pICMSST>
                            <vICMSST>0.18</vICMSST>
                        </ICMS70>
                    </ICMS>
                    <IPI>
                        <cEnq>999</cEnq>
                        <IPINT>
                            <CST>53</CST>
                        </IPINT>
                    </IPI>
                    <PIS>
                        <PISAliq>
                            <CST>01</CST>
                            <vBC>23.73</vBC>
                            <pPIS>1.65</pPIS>
                            <vPIS>0.39</vPIS>
                        </PISAliq>
                    </PIS>
                    <COFINS>
                        <COFINSAliq>
                            <CST>01</CST>
                            <vBC>23.73</vBC>
                            <pCOFINS>7.60</pCOFINS>
                            <vCOFINS>1.80</vCOFINS>
                        </COFINSAliq>
                    </COFINS>
                </imposto>
                <infAdProd>UN C/ 1 UN -ST: 0,18 -GTIN: 7506339337525</infAdProd>
            </det>
            <total>
                <ICMSTot>
                    <vBC>392.31</vBC>
                    <vICMS>78.45</vICMS>
                    <vICMSDeson>0.00</vICMSDeson>
                    <vFCPUFDest>0.00</vFCPUFDest>
                    <vICMSUFDest>0.00</vICMSUFDest>
                    <vICMSUFRemet>0.00</vICMSUFRemet>
                    <vBCST>382.00</vBCST>
                    <vST>9.84</vST>
                    <vProd>558.45</vProd>
                    <vFrete>0.00</vFrete>
                    <vSeg>0.00</vSeg>
                    <vDesc>0.00</vDesc>
                    <vII>0.00</vII>
                    <vIPI>0.00</vIPI>
                    <vPIS>9.20</vPIS>
                    <vCOFINS>42.43</vCOFINS>
                    <vOutro>1.98</vOutro>
                    <vNF>570.27</vNF>
                    <vTotTrib>0</vTotTrib>
                </ICMSTot>
            </total>
            <transp>
                <modFrete>0</modFrete>
                <transporta>
                    <CNPJ>05424008000441</CNPJ>
                    <xNome>UNILIDER DISTRIBUIDORA S.A - FILIAL RIO</xNome>
                    <IE>78362537</IE>
                    <xEnder>RODOVIA PRESIDENTE DUTRA, 2251 - GALPAO 1 ARM 101 E 102</xEnder>
                    <xMun>RIO DE JANEIRO</xMun>
                    <UF>RJ</UF>
                </transporta>
                <vol>
                    <qVol>5</qVol>
                    <esp>VOLUME(S)</esp>
                    <pesoL>12.587</pesoL>
                    <pesoB>13.689</pesoB>
                </vol>
            </transp>
            <cobr>
                <dup>
                    <nDup>864450</nDup>
                    <dVenc>2016-05-17</dVenc>
                    <vDup>570.27</vDup>
                </dup>
            </cobr>
            <infAdic>
                <infCpl>SIGLA: NLI PEDIDO:830396 ROTA:0006 - FARM Z OE I ROTEIRO:676373 NOME FANTASIA: FARMABELL|SO ACEITAMOS RECLAMACOES NO ATO DA ENTREGA. (FAVOR CONFERIR NA PRESENCA DO ENTREGADOR). FARMACIAS: ACEITAMOS RECLAMACOES ATE 24HS APOS A ENTREGA. SAC : 0800-755-0000 EMAIL: SAC@UNILIDER.COM.BR |WHATSAPP: (27) 99824-7116|SUBSTITUTO TRIBUTARIO - REG. TRIBUT. DIFERENCIADO - DEC.44.498 DE 29/11/2013. |REDUCAO DE BASE DE CALCULO CONF. ART. 2, INC. III.|VOLUMES: AL(1), NA(3), SC(1)|SUBSTITUTO TRIBUTARIO - REG. TRIBUT. DIFERENCIADO - DEC.44.498 DE 29/11/2013. |REDUCAO DE BASE DE CALCULO CONF. ART. 2, INC. III.|</infCpl>
            </infAdic>
        </infNFe>
        <Signature xmlns="http://www.w3.org/2000/09/xmldsig#">
            <SignedInfo>
                <CanonicalizationMethod Algorithm="http://www.w3.org/TR/2001/REC-xml-c14n-20010315" />
                <SignatureMethod Algorithm="http://www.w3.org/2000/09/xmldsig#rsa-sha1" />
                <Reference URI="#NFe33160405424008000441550010008644501143436782">
                    <Transforms>
                        <Transform Algorithm="http://www.w3.org/2000/09/xmldsig#enveloped-signature" />
                        <Transform Algorithm="http://www.w3.org/TR/2001/REC-xml-c14n-20010315" />
                    </Transforms>
                    <DigestMethod Algorithm="http://www.w3.org/2000/09/xmldsig#sha1" />
                    <DigestValue>NYP71ouK5Q1T9u6XiBWoYngeHpo=</DigestValue>
                </Reference>
            </SignedInfo>
            <SignatureValue>DFLespp7pgmWci1cfWQKIuYZGuvRZez+JsOfKNDP/i2UBOupnCPhjzegjvW6v8FTibj6Sk7VFS6ViitADKQMbUTP19q6C65ArHn+E/P9jDM7eJE1mdU+y+ji7ocIZ0QVrufhPHjd6eLZbtLaluyyFW2Veu1TI1izRzNH2SVUNx2tQwHzYuudChLPcLAMXf2UgdeFVjP1awrFMCal1HeQKJN8sLrAI5VU3um/2q5TBjhon0BnkpXn5EKiq+SBt4DW8GEpR8JBvUAZk98Aj0hxPjuw9eP90rD/rnfO63/HANGtvjM1/kt61HO0x13lX7PmGU88fL5BTtoPmjEHJBgZ+g==</SignatureValue>
            <KeyInfo>
                <X509Data>
                    <X509Certificate>MIIIRjCCBi6gAwIBAgIQZpj9R8GReV/JmhrFH2fikTANBgkqhkiG9w0BAQsFADB0MQswCQYDVQQGEwJCUjETMBEGA1UEChMKSUNQLUJyYXNpbDEtMCsGA1UECxMkQ2VydGlzaWduIENlcnRpZmljYWRvcmEgRGlnaXRhbCBTLkEuMSEwHwYDVQQDExhBQyBDZXJ0aXNpZ24gTXVsdGlwbGEgRzUwHhcNMTUwNjAzMDAwMDAwWhcNMTYwNjAxMjM1OTU5WjCByzELMAkGA1UEBhMCQlIxEzARBgNVBAoUCklDUC1CcmFzaWwxIjAgBgNVBAsUGUF1dGVudGljYWRvIHBvciBBUiBBQ0UgRVMxGzAZBgNVBAsUEkFzc2luYXR1cmEgVGlwbyBBMTEVMBMGA1UECxQMSUQgLSA4MzE3NDAyMSMwIQYDVQQDExpVTklMSURFUiBESVNUUklCVUlET1JBIFMgQTEqMCgGCSqGSIb3DQEJARYbam9hby52aWN0b3JAdW5pbGlkZXIuY29tLmJyMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEApMSVlD8yZV9BNekonEtF+qBp4ei5v+nP6JiyYyD9ei+4EOIoN5OqX3gIAPym3sC31roaIOlcUtviSZC8s3lzAWJJFRXfGjHeK+N6/epxZucxZKvNLXmcxJL1ROvd32pYRFQROUKh2d7/aPM2K1cQQihYregQbAYTMYKaWBjXB3ZNs6tyEXYO3X3kdcnNDrR+ZECPpbISAbEB6p37V6JXbnPKzBEVPY39ADA7na6T4vPuUa+tKgPtas3NJoKmWkZyH/haUPqnUoV9feAcpsAlcXOg2BgfT+5TNlaK5xmpoKurGFpd2nI1BBJmFjzu21CcmrSAI5/LbZ5BnyTTVZAPOwIDAQABo4IDejCCA3YwgcAGA1UdEQSBuDCBtaA+BgVgTAEDBKA1BDMwMzA1MTk5MzEzNjM4NTExNzkwMDAwMDAwMDAwMDAwMDAwMDAwMDMwNDgyMDRTUFRDRVOgIgYFYEwBAwKgGQQXSm9hbyBWaWN0b3IgZGUgT2xpdmVpcmGgGQYFYEwBAwOgEAQOMDU0MjQwMDgwMDA0NDGgFwYFYEwBAwegDgQMMDAwMDAwMDAwMDAwgRtqb2FvLnZpY3RvckB1bmlsaWRlci5jb20uYnIwCQYDVR0TBAIwADAfBgNVHSMEGDAWgBSdUM+9/yTKr7Ez6xfiQnqOaSqOUzAOBgNVHQ8BAf8EBAMCBeAwgYkGA1UdIASBgTB/MH0GBmBMAQIBCzBzMHEGCCsGAQUFBwIBFmVodHRwOi8vaWNwLWJyYXNpbC5jZXJ0aXNpZ24uY29tLmJyL3JlcG9zaXRvcmlvL2RwYy9BQ19DZXJ0aXNpZ25fTXVsdGlwbGEvRFBDX0FDX0NlcnRpU2lnbk11bHRpcGxhLnBkZjCCASUGA1UdHwSCARwwggEYMFygWqBYhlZodHRwOi8vaWNwLWJyYXNpbC5jZXJ0aXNpZ24uY29tLmJyL3JlcG9zaXRvcmlvL2xjci9BQ0NlcnRpc2lnbk11bHRpcGxhRzUvTGF0ZXN0Q1JMLmNybDBboFmgV4ZVaHR0cDovL2ljcC1icmFzaWwub3V0cmFsY3IuY29tLmJyL3JlcG9zaXRvcmlvL2xjci9BQ0NlcnRpc2lnbk11bHRpcGxhRzUvTGF0ZXN0Q1JMLmNybDBboFmgV4ZVaHR0cDovL3JlcG9zaXRvcmlvLmljcGJyYXNpbC5nb3YuYnIvbGNyL0NlcnRpc2lnbi9BQ0NlcnRpc2lnbk11bHRpcGxhRzUvTGF0ZXN0Q1JMLmNybDAdBgNVHSUEFjAUBggrBgEFBQcDAgYIKwYBBQUHAwQwgaAGCCsGAQUFBwEBBIGTMIGQMGQGCCsGAQUFBzAChlhodHRwOi8vaWNwLWJyYXNpbC5jZXJ0aXNpZ24uY29tLmJyL3JlcG9zaXRvcmlvL2NlcnRpZmljYWRvcy9BQ19DZXJ0aXNpZ25fTXVsdGlwbGFfRzUucDdjMCgGCCsGAQUFBzABhhxodHRwOi8vb2NzcC5jZXJ0aXNpZ24uY29tLmJyMA0GCSqGSIb3DQEBCwUAA4ICAQBLeNl6dAohkszu05/+v+RwX9G4rpSpDbHCyA3BuBBlLDzUTwvxuIMtMeBLw0LQdRh3cKOeNZLbnSaXL22aMq6F8fS85YqHB1fHWPFDZgR1cwJEBOE2GxrMrcKqDx3QkJV09rWcU0M3OlzbjoydKlFEXCW2rvgQWpqsaA8P6oXd+hDMLcsyXCGd3WxZARjz+yv2aQ8EE/TlYmkD07Y1quaY1rZlcTZAbxWcirR+1RKQps9uutT60oqnFR2BXsY16o5vLDnTgT0zFwiaVokMtmmlZJ4T9hLCv7kOJTPmFFYwviym4x7kBXnXD+OVYUVv0yFZKfA6wbo+PppCoY6uIzsoLybGLGL6/UD9Ygqvd6OE2ir5phVJadRxDW2J7YvSDtTz2ECpoW1igFD9kqgAtOKGIlo4OdFO+aPLaXOSz5vwM5OSGOxMSeU21yvlJK1K3TuiOeTi4OhRrgszs6nUwT1BwAqCbLGDk+OeqOgos8Lg8TIS+IvdIjme4Q2O6vNPV0qs0v5jbyxaVhtCkOCluedeol3JpV+ysvMojY0TmGaVvEMsPI1uTw1uICK3xy2QZyE8wHdkXh+bWg16ovjwqVWweucqA9dSgH2//3RDWd7K5xPNV3MXFfDSzQGQVFuSpXZXM3ym8fWpxf/7OzR7qXN9pShWRFwXtb8j+FubeEB+Tw==</X509Certificate>
                </X509Data>
            </KeyInfo>
        </Signature>
    </NFe>
    <protNFe versao="3.10">
        <infProt>
            <tpAmb>1</tpAmb>
            <verAplic>3.10</verAplic>
            <chNFe>33160405424008000441550010008644501143436782</chNFe>
            <dhRecbto>2016-04-26T09:07:51-03:00</dhRecbto>
            <nProt>333160053773135</nProt>
            <digVal>NYP71ouK5Q1T9u6XiBWoYngeHpo=</digVal>
            <cStat>100</cStat>
            <xMotivo>Autorizado o uso da NF-e</xMotivo>
        </infProt>
    </protNFe>
</nfeProc>
```

# Requisitos

# Certificado Digital

# Computador

# Software

# Internet

# Campos obrigatórios e como preenchê#los:

# Dados do Emitente (você)

# Dados do Destinatário (seu cliente)

# Produto(s) ou Serviço(s) vendido(s)

# Nome do Produto ou Serviço

# Tipo

# Quantidade

# Valor Unitário

# Valor Total

# Peso Líquido Total

# Peso Bruto Total

# NCM

# CEST (Código Especificador de Substituição Tributária)

# Tributação:

# ICMS

# Situação Tributária

# Origem

# Natureza da operação

# Forma de pagamento

# CFOP (Códigos Fiscais de Operações e Prestações)

# Base de Cálculo do ICMS

# Valor Total do ICMS

# Base de Cálculo do ICMS ST

# Valor Total do ICMS ST

# Valor Total dos produtos e serviços

# Valor Total do Frete

# Valor Total do Seguro

# Valor Total do Desconto

# Outras Despesas acessórias

# Valor Total da NF-e

# Valor aproximado total de tributos federais, estaduais e municipais

