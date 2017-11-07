String codProd = labelCodProd.getText().trim();
        String cliente = labelCliente.getText().trim();
       
        DefaultTableModel validacao = (DefaultTableModel)TableVendas.getModel();
        validacao.addRow(new String[] {codProd, cliente});
        
        labelCodProd.setText(TextCodProd.getText());
        labelCliente.setText(TextCliente.getText());
        
        labelCodProd.requestFocus();


---------------------------------------------------------------------------------------
objeto para validação:

Object[] row = new Object[5];
                row[0] = cli.getId();
                row[1] = cli.getNome();
                row[2] = cli.getSobrenome();
                row[3] = cli.getDataNascimento();
                row[4] = cli.getGenero();
                model.addRow(row);
