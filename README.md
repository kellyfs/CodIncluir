String codProd = labelCodProd.getText().trim();
        String cliente = labelCliente.getText().trim();
       
        DefaultTableModel validacao = (DefaultTableModel)TableVendas.getModel();
        validacao.addRow(new String[] {codProd, cliente});
        
        labelCodProd.setText(TextCodProd.getText());
        labelCliente.setText(TextCliente.getText());
        
        labelCodProd.requestFocus();
